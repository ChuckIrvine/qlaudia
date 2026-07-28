# Prior Art Scan — Summary (New Claim Families for Non-Provisional: Inventions 3–5, plus refinements to Inventions 1–2)

**Scope:** Lightweight scan (not a substitute for a formal search) covering subject matter added to the non-provisional that was not in the original provisional: (3) two-phase LLM-generated relationship-type vocabulary + archetype-classified structural edges, (3a) deterministic prerequisite-cycle resolution + zero-prerequisite diagnostic, (2a) importance/centrality-tie-broken topological goal-path construction to an arbitrary user-selected topic, (4) bounded-turn conversational AI course-brief elicitation, (5) dual-mode hybrid semantic search (domain-tagline + concept embeddings, LLM reranking, threshold gating) over an AI-generated KB.

---

## Invention 3 — Two-Phase Structural Relationship-Type Generation

**Key novelty emphasis:** the two-call design (Call 1 derives a bounded, archetype-classified relationship-type *vocabulary* from the full corpus of generated docs; Call 2 assigns edges from that vocabulary, batched, with post-hoc validation dropping hallucinated endpoints/self-loops/duplicates) is the differentiator — not "LLM extracts relationships from text," which is well-trodden.

**Findings:** General LLM-based knowledge-graph relation extraction and relation-type prediction are well established in patent and academic literature (e.g., US20250112878A1 "Knowledge graph assisted large language models," US20250131289A1 "Knowledge Graph Extraction," US11798529B2). None of the surveyed references disclose a **corpus-derived, archetype-classified relationship-type vocabulary generated in a first pass and then constrained-assigned in a second pass with automated hallucination/self-loop/duplicate filtering**, specifically applied to an AI-generated educational KB. This two-phase vocabulary-then-assignment structure, plus the archetype taxonomy (functional/hierarchical/causal/spatial/temporal/safety/other), appears to be a reasonable differentiator.

**Novelty opportunity:** claim the two-phase vocabulary-derivation-then-edge-assignment method as a distinct step sequence, with the validation/filtering step as a dependent claim.

---

## Invention 3a — Deterministic Prerequisite-Cycle Resolution + Zero-Prerequisite Diagnostic

**Findings:** Cycle detection/removal in DAGs is a generic, well-known graph-theory technique (see general DAG cycle-resolution literature). No prior art was found applying a **deterministic, pedagogically-informed** cycle-breaking rule (removing the edge whose source concept is more "advanced" relative to the target) specifically to LLM-generated prerequisite graphs, nor a **secondary LLM diagnostic pass** that re-examines any concept left with zero prerequisites to confirm it is genuinely foundational rather than a generation gap.

**Novelty opportunity:** claim the combination — deterministic advancement-based cycle resolution + LLM-driven zero-prerequisite re-diagnosis — as a validation sub-step of KB generation (Invention 1), not a standalone invention.

---

## Invention 2a — Importance-Weighted Goal-Directed Topological Pathing

**Findings:** The closest identified reference is **US 9,189,968 B1 / US 9,672,470 B2 ("Network-probability recommendation system," Pearson Education, filed 2013)**, which recommends a next node in a prerequisite graph using a *probabilistic* likelihood-of-success model based on the user's interaction history — not a deterministic topological sort to an arbitrary selected goal node, and not centrality/importance-based tie-breaking. Academic work on course-prerequisite networks applies centrality measures (betweenness, in/out-degree) descriptively, to identify "hub"/"bottleneck" courses, but not as a **tie-breaker inside a per-user, on-demand topological sort of the transitive-prerequisite subgraph of an arbitrarily chosen target topic**.

**Novelty opportunity:** claim (a) on-demand construction of an ordered learning path to *any* user-selected (not pre-set) topic by topologically sorting its transitive-prerequisite subgraph, and (b) using a graph-centrality importance score as the deterministic tie-break, as a refinement/dependent claim under Invention 2 (Adaptive Learning Framework) — not a standalone invention, since it extends the same "goal-directed pathfinding" claim already in the provisional.

---

## Invention 4 — Bounded-Turn Conversational AI Course-Brief Elicitation

**Findings:** No patent references were found disclosing a bounded-turn (max-N-questions), multi-modal-attachment-accepting conversational agent whose specific purpose is to produce a **structured brief with fixed fields** (target audience, coverage overview, desired outcome, tone/style) that is then used as direct input to an automated KB-generation pipeline. General "use a chatbot to help write a syllabus" content exists only as informal/consumer guidance (blog posts, prompt libraries), not as a claimed system architecture tying the interview output schema to a downstream generation pipeline.

**Novelty opportunity:** claim the conversational interview as a front-end method step of Invention 1 — bounded turns, multi-modal ingestion, and a fixed structured-output schema that feeds concept discovery — framed as a data-acquisition method rather than "a chatbot," to avoid abstract-idea rejection risk.

---

## Invention 5 — Hybrid Semantic Search Over an AI-Generated KB

**Findings:** Vector-embedding search plus LLM/cross-encoder reranking ("hybrid search + rerank") is a widely known and increasingly commoditized RAG pattern with substantial prior art and non-patent literature (no shortage of implementations). The specific combination claimed here — **two independent embedding indexes (domain-tagline embeddings for course discovery, concept embeddings for in-course search), each with its own similarity threshold gate, over a KB whose content was itself generated by the same pipeline as Invention 1** — is narrower than generic "RAG search," but the underlying retrieve+rerank+threshold mechanism itself is likely to face strong prior art headwinds if claimed broadly.

**Novelty opportunity / caution:** claim narrowly — specifically the dual-index (domain vs. concept) architecture with independent thresholds operating over a KB produced by Invention 1's generation pipeline — rather than the general retrieve-then-rerank pattern, which is unlikely to be allowed on its own. Consider this claim set the weakest of the five and a candidate to trim first if the application needs to shrink.

---

## Recommendation Carried Into Drafting
- Fold Invention 2a (goal-pathing) in as a dependent claim under Claim Set 2, and Invention 3a (cycle resolution) in as a dependent claim under Claim Set 1 — per the task plan, these are refinements, not standalone claim sets.
- Draft Claim Set 3 (relationship-type generation), Claim Set 4 (conversational elicitation), and Claim Set 5 (hybrid search) as independent claim families, with Claim Set 5 drafted narrowly per the caution above.

---

## Invention 6 — Interactive Mastery-Aware Knowledge Graph Navigation

**Added during the section-by-section review**, after the initial draft — this feature (`ConceptNeighborhoodGraph.tsx`, `app/api/neighborhood/route.ts`) was not caught in the original codebase survey's scoping pass.

**Findings:** The closest identified reference is **US 8,909,653 B1 / US 8,832,117 B2 / US 2014/0356846 A1 ("Apparatus, systems and methods for interactive dissemination of knowledge," Julius Su)**, which discloses a GUI limiting a displayed knowledge-graph view to items directly connected to nodes on a learning path, and single-metric shading to indicate understanding level. It does not disclose: a four-state mastery-relative coloring scheme computed from a separate adaptive-learning-framework readiness/recommendation determination (mastered / recommended-next / ready / not-yet-ready); click-to-recenter node-by-node graph traversal (its interactivity is drag-and-drop learning-path editing, a different mechanism than re-centering a neighborhood view); importance/centrality-based top-K neighbor filtering with a numeric rank indicator; or natural-language relationship descriptions surfaced on hover/tap.

**Novelty opportunity / caution:** the generic idea of "show only directly-connected graph items" is already disclosed by the Su reference, so Claim Set 6 must be drafted around the specific combination above, not the bare neighborhood-limiting idea. As drafted, claim 23 requires the four-state mastery-relative coloring *and* the click-to-recenter traversal together; claims 24 and 26 add the importance-ranked filtering and relationship-description interaction as further narrowing dependent limitations.

## Recommendation Carried Into Drafting (Invention 6)
- Draft Claim Set 6 as an independent claim family, scoped narrowly around the combination of mastery-relative coloring, click-to-recenter traversal, importance-ranked filtering, and relationship-description interaction, to distinguish over the Su reference.
