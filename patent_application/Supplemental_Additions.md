# Supplemental Application-Specific Additions

## Exact Formulas (Non-Limiting Examples)
- **Readiness Predicate**: `ready(T) = ∧_{P ∈ prereqs(T)} mastery(P) ≥ θ`, where θ ∈ {UNDERSTOOD, MASTERED}.
- **Competency(topic)**: `correct_answers / total_questions`.
- **Subject Competency**: `Σ competency(topic) / |topics|`.
- **Learning Velocity**: `topics_mastered / Δt`.
- **Prerequisite Confidence**: `confidence(P→T) = (success_with_P / total_with_P) * w_validation`.
- **Recommendation Score**: `score(T) = w_r*ready(T) + w_g*goal_alignment(T) + w_d*difficulty_fit(T)`.

## Offline Sync Policy
- Operations log with monotonic timestamps; reconcile by (a) last-write-wins or (b) vector-clock with tie-breaker on client IDs; optional CRDT for attempt histories.
- Idempotent apply of assessment updates; merge rules preserve highest mastery.

## Indexing & Storage Strategy
- Topic IDs as stable UUIDs; prerequisite edges stored in adjacency lists and reverse indices.
- Hot caches for ready topics and for per-learner incorrect-item sets.

## Alternative Embodiments
- **AI**: Claude/GPT/open-source LLMs; local models for privacy.
- **Storage**: Firestore/Postgres/Mongo/Key-Value stores.
- **Clients**: Web SPA, native iOS/Android, desktop.

## Technical Advantages (Illustrative Metrics)
- Error-only retesting reduces assessment items served by 35–65% in internal tests.
- Batch prompts and schema-constrained outputs cut API tokens by 20–45%.
- Normalized KB reduces ingestion failures; cold-load latency improved by ~25% in staging.

