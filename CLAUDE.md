# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Structure

Qlaudia is an AI-powered learning platform with two independent sub-projects:

- **`qlaudia_ui/`** — Next.js 15 frontend (App Router, TypeScript, Tailwind CSS)
- **`qlaudia_server/`** — FastAPI backend (Python 3.13, LangGraph, Neo4j)

These are developed and deployed independently. There is no shared package or monorepo tooling tying them together.

---

## qlaudia_ui (Next.js Frontend)

### Commands

```bash
cd qlaudia_ui
npm run dev          # start dev server on :3000
npm run build        # production build
npm run lint         # ESLint

npm run env:dev      # switch to local .env.local (points to local Neo4j + local FastAPI)
npm run env:prod     # switch to prod .env.local (points to prod Neo4j + prod FastAPI)
```

### Architecture

**Routing:** Next.js App Router. `app/page.tsx` is the splash screen (shown to signed-out users). `app/domains/page.tsx` is the main app shell.

**Authentication:** Clerk (`@clerk/nextjs`). `useUser()` and `useAuth()` hooks in components; `auth()` and `currentUser()` in server-side API routes. `isSignedIn` gates most UI features.

**Database access:** Neo4j is queried directly from Next.js API routes via `lib/neo4j.ts`. There is no ORM — raw Cypher queries are written inline.

**State management:** Zustand stores in `store/`:
- `graphStore` — graph data, selected node/edge
- `domainStore` — active domain, concept list
- `userStore` — current user and progress
- `preferencesStore` — dark mode, etc.

**API routes** (`app/api/`): Each folder is a REST endpoint. Key ones:
- `auth/me` — resolves Clerk user, creates Neo4j user node, returns `canCreateDomain` and `editableDomains`
- `search` — Voyage AI `voyage-3` embedding → Neo4j vector search → Voyage AI `rerank-2-lite` reranker (0.55 threshold)
- `concepts` — fetch concept content, progress, prerequisites
- `progress` — track known/unknown concepts
- `graph` — full graph query for GraphCanvas visualization
- `neighborhood` — immediate neighbors of a concept
- `domains/create/*` — SSE stream proxied to FastAPI

**Permissions:**
- `DOMAIN_CREATOR_IDS` env var (comma-separated Clerk user IDs) controls who can create domains
- `EDITOR_PERMISSIONS` env var (format: `userId:domain1,domain2;userId2:*`) controls who can edit concepts

**Key components:**
- `AppShell.tsx` — top nav, domain selector, dark mode, feedback, mobile menu
- `DomainBrowser.tsx` — main learning UI (concept list sidebar + content panel)
- `CreateDomainModal.tsx` — multi-step domain creation via FastAPI SSE
- `GraphCanvas.tsx` — knowledge graph visualization

**Important Next.js note (from AGENTS.md):** This version may have breaking changes from training data. Read `node_modules/next/dist/docs/` before writing Next.js-specific code.

---

## qlaudia_server (FastAPI Backend)

### Commands

```bash
cd qlaudia_server
python3.13 -m venv .venv
.venv/bin/pip install -e .           # install dependencies
cp .env.example .env                 # fill in keys

.venv/bin/python start_fast_api.py   # start API on :8000 with hot reload
```

### Architecture

**Domain creation pipeline** (`src/domain_creation_pipeline/`): A LangGraph `StateGraph` that runs these steps sequentially:

1. `step1_concept_map.py` — LLM generates concept list (runs separately before pipeline, user reviews)
2. `step3_atomic_docs.py` — generates markdown doc per concept (batched, primary LLM)
3. `step3b_qa.py` — generates quiz Q&A per concept (QA LLM, Haiku)
4. `step4_edges.py` — generates concept relationship edges (primary LLM, max_tokens=32000)
5. `step5_prerequisites.py` — generates prerequisite edges (primary LLM, max_tokens=32000)
6. `step9_embeddings.py` — Voyage AI `voyage-3` embeddings
7. `step10_graph_population.py` — writes everything to Neo4j

**Two graph functions in `graph.py`:**
- `build_phase2_pipeline()` — flat graph for FastAPI streaming (used by API server)
- Nested subgraph version — used by CLI script `scripts/domain/create_domain_kg.py`

**LLM configuration** (`src/domain_creation_pipeline/models.py`):
- Primary role (steps 1, 3): `claude-sonnet-4-6` (default) or Groq `llama-3.3-70b-versatile` via `PRIMARY_LLM_PROVIDER=groq`
- QA role (step 3b): `claude-haiku-4-5-20251001` (default) via `QA_LLM_PROVIDER`
- Steps 4 and 5 always use Claude directly (bypass the factory)

**FastAPI server** (`src/api/main.py`):
- In-memory job store (`_jobs` dict) tracks pipeline runs by job ID
- Pipeline runs as `asyncio.create_task` (cancellable via DELETE endpoint)
- Progress streamed to UI via SSE (`EventSourceResponse`)

**Neo4j data model:**
- `Concept` nodes with `name`, `tagline`, `content` (markdown), `importance` (betweenness centrality 0–1), embedding vector
- `Domain` nodes linked to concepts
- `PREREQUISITE_FOR` edges — "prereqs" always means transitive (`[:PREREQUISITE_FOR*]`)
- Named relationship types (e.g., `RELATED_TO`, domain-specific types) stored as separate edge types

### Key scripts (run from `qlaudia_server/`)

```bash
.venv/bin/python scripts/domain/create_domain_kg.py   # full CLI pipeline (pauses for concept review)
.venv/bin/python scripts/domain/delete_domain.py -local
.venv/bin/python scripts/domain/migrate_to_prod.py --domain "Domain Name"
```

---

## Environment Variables

### qlaudia_ui (.env.local)
- `NEO4J_URI`, `NEO4J_USERNAME`, `NEO4J_PASSWORD`, `NEO4J_DATABASE`
- `VOYAGE_API_KEY`
- `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`
- `DOMAIN_CREATOR_IDS` — comma-separated Clerk user IDs allowed to create domains
- `EDITOR_PERMISSIONS` — `userId:domain1,domain2;userId2:*`
- `NEXT_PUBLIC_FASTAPI_URL` — URL of the FastAPI server

### qlaudia_server (.env)
- `NEO4J_URI`, `NEO4J_USERNAME`, `NEO4J_PASSWORD`
- `ANTHROPIC_API_KEY`, `VOYAGE_API_KEY`
- `GROQ_API_KEY` (optional, for Groq LLM)
- `PRIMARY_LLM_PROVIDER` — `anthropic` (default) or `groq`
- `QA_LLM_PROVIDER` — `anthropic` (default) or `groq`
- `ALLOWED_ORIGINS` — comma-separated CORS origins (default: `http://localhost:3000`)

---

## Deployment

- **Frontend:** Vercel (auto-deploys from main branch)
- **Backend:** Render (`qlaudia_server/render.yaml`). Only redeploys when `src/`, `pyproject.toml`, `render.yaml`, or `.python-version` change (configured via `ignoreCommand`).
