# Information Disclosure Statement — Reference List

Prepared for filing alongside the non-provisional application (`non_provisional_patent_app.md`), claiming priority to Provisional Application No. 63/864,273 (filed 2025-08-14). This list compiles every prior-art reference identified across the provisional's own prior-art scans and this session's supplemental scan for the new claim families. It is intended as the source list for USPTO Form SB/08 (Information Disclosure Statement) — transcribe the entries below onto the current version of that form (or its Patent Center equivalent) when filing.

**Note:** this is a compiled research list, not a substitute for your own or counsel's independent judgment on materiality. Include any reference you are independently aware of that isn't listed here.

---

## U.S. Patents and Published Applications

| # | Reference | Relevance |
|---|---|---|
| 1 | US 11,645,095 B2 (2023) | Builds tutorial knowledge graphs; cited against Claim Set 1 (KB generation) — lacks schema standardization and prompt-based AI generation. |
| 2 | US 2023/0351102 A1 | General AI document generation; cited against Claim Set 1 — not course-specific, no canonical schema. |
| 3 | US 2023/0259705 A1 | Structured data transformations; cited against Claim Set 1 — no AI generation pipeline from prompts. |
| 4 | US 10,490,092 B2 (2019) | Mastery-learning platform with knowledge maps; cited against Claim Set 1 (no AI-generated KB) and Claim Set 2 (prerequisite graph, goal-directed pathing, mastery gating — closest reference on those elements, but no targeted re-testing of incorrect items). |
| 5 | US 11,403,565 B2 (2022) | Learning paths from structured graphs; cited against Claim Set 1 and Claim Set 2 — prerequisite/goal pathing present, mastery gating partial, no targeted re-testing. |
| 6 | US 7,052,277 B2 (2006) | Early adaptive sequencing system; cited against Claim Set 2 — partial prerequisite graph and goal pathing, mastery gating present, no targeted re-testing. |
| 7 | US 2019/0226868 A1 | Goal/prerequisite graphs for adaptive learning; cited against Claim Set 2 — re-testing not specified. |
| 8 | US 2022/0327946 A1 | Skills-hierarchy tracking system; cited against Claim Set 2 — mastery gating present, re-testing logic not described. |
| 9 | US 9,189,968 B1 ("Network-probability recommendation system," Pearson Education, filed 2013) | **Closest identified reference to Claim Set 2's goal-directed path construction.** Discloses a prerequisite graph with recommendation of a next node based on a probabilistic likelihood-of-success model from user interaction history. Does not disclose deterministic topological sorting to an arbitrary user-selected goal node, nor centrality/importance-based tie-breaking. |
| 10 | US 9,672,470 B2 (same family as #9, Pearson Education) | Same relevance as #9. |
| 11 | US20250112878A1 ("Knowledge graph assisted large language models") | Cited against Claim Set 3 (structural relationship generation) — general LLM-assisted knowledge-graph construction; no two-phase vocabulary-then-assignment method or archetype classification. |
| 12 | US20250131289A1 ("Knowledge Graph Extraction") | Cited against Claim Set 3 — general knowledge-graph extraction; same distinction as #11. |
| 13 | US11798529B2 ("Generation of optimized knowledge-based language model through knowledge graph multi-alignment") | Cited against Claim Set 3 — general KG/LLM alignment technique; no relationship-type vocabulary generation step. |
| 16 | US 8,909,653 B1 / US 8,832,117 B2 / US 2014/0356846 A1 ("Apparatus, systems and methods for interactive dissemination of knowledge," Julius Su) | **Closest identified reference to Claim Set 6 (interactive graph navigation).** Discloses a GUI limiting a displayed knowledge-graph view to items directly connected to nodes on a learning path, and single-metric shading to indicate understanding level. Does not disclose: a four-state mastery-relative coloring scheme tied to an adaptive-learning-framework readiness/recommendation computation; click-to-recenter node-by-node graph traversal (its interactivity is drag-and-drop learning-path editing, not neighborhood re-centering); importance/centrality-based top-K neighbor filtering with a rank indicator; or natural-language relationship descriptions on hover/tap. Claim Set 6 is drafted narrowly around this combination to distinguish over this reference. |

## Non-Patent Literature

| # | Reference | Relevance |
|---|---|---|
| 14 | Course-prerequisite-network research applying centrality measures (betweenness, in/out-degree) to identify hub/bottleneck courses (e.g., academic literature on "Course-Prerequisite Networks" and centrality analysis of curriculum graphs) | Cited against Claim Set 2's importance-score tie-breaking — centrality measures are used descriptively in this literature to characterize course networks, not as a deterministic tie-break inside a per-user, on-demand topological sort to an arbitrary goal. |
| 15 | General retrieval-augmented-generation ("RAG") literature on hybrid vector search + reranking (dense retrieval + cross-encoder/LLM rerank pipelines) | Cited against Claim Set 5 (hybrid semantic search) — the general retrieve-then-rerank pattern is widely known; Claim Set 5 is drafted narrowly around the dual-index (domain-tagline vs. topic-content), independently-thresholded architecture specifically to distinguish over this broad body of art. |

---

## Filing Notes
- References 1–8 originate from the provisional's own prior-art scans (`prior_art_scan_inv1_summary_redo.md`, `prior_art_scan_inv2_summary.md`, `prior_art_comparison_inv1_redo.md`, `prior_art_comparison_inv2.md`).
- References 9–15 originate from this session's supplemental scan (`prior_art_scan_inv3_5_summary.md`) for the newly added claim families.
- Reference 16 was identified during the section-by-section review, when Claim Set 6 (interactive graph navigation) was added after the initial draft.
- This was a lightweight web/patent-database scan, not a formal, paid prior-art search. If a formal search is later commissioned (e.g., during prosecution), any additional material references it turns up should be disclosed via a supplemental IDS.
- USPTO IDS filing requires either (a) filing within 3 months of the non-provisional's filing date / before first Office Action (no fee), or (b) later, with a fee and/or a statement of when the reference first became known, per 37 CFR 1.97–1.98. File this IDS with the initial application to use the no-fee window.
