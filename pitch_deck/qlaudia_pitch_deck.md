# Qlaudia — Angel Investor Pitch Deck

> **Status:** v0.2 draft. Retuned for **angel investors** (individuals and syndicates writing $25K–$250K checks).
> **Markdown is the source of record; PowerPoint conversion to follow.**
>
> **Convention:** each `##` heading is one slide. `**Headline:**` is the on-slide assertion.
> Body bullets are on-slide text. `> Speaker notes:` blocks do not appear on the slide.
> `⚠️ TODO` marks content that needs Charles's input before this goes in front of investors.
>
> **Design target:** 13 slides, ~12 minutes, then questions. Angels stop absorbing after about
> a dozen slides. Everything diligence-grade lives in the appendix and gets sent *after* the meeting.

---

## Slide 1 — Education Is the Largest Untransformed Market on Earth

**Headline:** $7.3 trillion is spent teaching people every year. It is the last great industry whose product is still made entirely by hand.

### Education is the second-largest sector of human activity on Earth

| Sector | Annual global spend | Source |
|---|---|---|
| Healthcare | $9.8T *(2022)* | WHO — 9.9% of global GDP |
| **Education & training** | **$7.3T** *(2025)* | HolonIQ |
| All IT spending worldwide | $5.43T *(2025)* | Gartner |
| All military spending worldwide | $2.72T *(2024)* | SIPRI |

**Larger than the entire global IT industry. Roughly 2.7× the world's combined military spending.**

### The whole of education and training — global annual expenditure

| Segment | Annual spend | Notes |
|---|---|---|
| **Global education & training, all segments** | **~$7.3T (2025) → ~$10T (2030)** | HolonIQ; 4.4% CAGR |
| K–12 / primary & secondary (global) | ~$2.5T | Largest single block by headcount |
| Higher education (global) | ~$2.2T | |
| Workforce, corporate & vocational training | ~$400B+ | Fastest-growing segment |
| Early childhood | ~$400B+ | Fastest-growing segment |
| **Global EdTech (digital slice of the above)** | **~$404B (2025)** | Only ~5.5% of total education spend is digital |

### Adjacent spend that is really education spend

Private tutoring (~$134B global) · Corporate training (~$427B global) · Language learning (~$85B global) · Test prep & admissions · Professional licensure & continuing education (CME, CLE, CPE, bar, nursing, trades) · IT & technical certification · Homeschooling, microschools & pods · Compliance & regulatory training · Military, government & NGO training · Self-directed learning & bootcamps · Textbook & courseware publishing

### The three numbers that matter

1. **~$7.3T** — total annual spend on teaching human beings. Growing to **$10T by 2030**.
2. **~5%** — the share of that spend that is digital today. The other 95% is people, buildings, and paper.
3. **$0** — the amount currently going to a system that can generate a *rigorous, prerequisite-structured, verifiable knowledge graph* for any subject on demand.

> **Speaker notes:**
> **U.S. figures, if an American angel wants them (full table in Appendix A8):** K–12 public schools ~$1.0T in FY2024, the first year over a trillion, ~$17.6K per pupil. Higher education ~$712B. Corporate training ~$100B. Private tutoring ~$30B and growing double digits.
>
> Say out loud, before anyone else says it: *"No company captures a market this size, and I'm not going to pretend otherwise."* Saying it first converts the deck's biggest liability into a credibility marker. Then land the actual point, which is **structural, not arithmetic**: education is the last enormous market where the core product — a coherent, sequenced body of knowledge taught in the right order — has never been *manufacturable*. It's hand-built by humans, one course at a time. That's why it costs what it costs. Qlaudia makes the knowledge itself manufacturable.
>
> Then immediately promise the follow-through: *"Slide 9 shows the specific slice I'm going after first, and what it's worth."* An angel who hears a $7.3T number and never hears a reachable number assumes you can't tell the difference. Don't leave that gap open across eight slides.
>
> Anticipated pushback: *"EdTech is a graveyard."* Correct — because prior EdTech sold *delivery* (an LMS, a video player, a quiz engine) into institutions that already had content. Qlaudia sells the content layer itself, which is the expensive part.
>
> **The capital-gap stat — hold this in reserve, do not volunteer it.** Digital health VC is on track for ~$28B in 2025. EdTech VC was ~$2.4B in 2024, a decade low, and Q1 2025 fell another 35%. Normalized against sector size, healthcare draws roughly **9× more venture capital per dollar of sector spending** than education does — a market three-quarters the size of healthcare attracting one-twelfth the venture dollars.
>
> This stat cuts both ways and the framing decides which. Volunteered cold it reads as *"the market has spoken and it said no."* Deployed as the answer to "isn't EdTech a graveyard?" it is devastating: *"Yes — and that's why I can build a healthcare-scale company with no competition for capital or talent. The graveyard is full of companies that sold delivery. I sell the content."* Say it only after you've named why the prior generation failed.
>
> **Year alignment — be precise if pressed.** WHO's latest global health figure is 2022 ($9.8T); healthcare today is likely ~$11T. Against a 2025 education number, the honest ratio is closer to two-thirds than three-quarters. The years are labelled on the slide for exactly this reason — don't let a sharp angel be the one to point it out.

---

## Slide 2 — The Problem

**Headline:** Building a course is still artisanal. That's why education doesn't scale, doesn't adapt, and doesn't transfer.

- **Content is hand-built.** A single university course takes an expert months. A curriculum takes years. Cost scales linearly with subjects covered.
- **Structure is implicit.** Prerequisites live in a professor's head or a syllabus footnote — not in a machine-readable form anything can reason over.
- **Sequencing is one-size-fits-all.** Everyone walks the same path at the same pace regardless of what they already know.
- **AI chatbots don't fix this.** An LLM answers any question fluently, but it has no model of *what you know*, *what you must learn first*, or *whether the explanation it just gave was correct*. It tutors without a curriculum.

> **Speaker notes:**
> The chatbot bullet is the one that matters. Every angel in the room has already used ChatGPT to learn something and has a private opinion about how well it went. Make the distinction concrete: a chatbot is a conversation that evaporates; Qlaudia is a structured, persistent, verifiable body of knowledge that a conversation can stand on.
>
> **Optional setup for Slide 4.** If you want the founder slide to detonate, plant the fuse here: "the hand-authoring bottleneck isn't new — it's the reason this whole approach was abandoned forty years ago." Then let Slide 4 reveal that you were one of the people who hit that wall and wrote it down.

---

## Slide 3 — The Solution

**Headline:** Qlaudia generates a complete, prerequisite-structured knowledge graph for any subject — in hours, not months — and teaches from it adaptively.

**Two inventions, independently valuable:**

1. **Knowledge base generation.** Point Qlaudia at a subject. It produces a graph of concepts, each with written instruction, computed figures, worked examples, and assessments — plus the typed relationships and prerequisite edges that connect them.
2. **Adaptive, goal-directed delivery.** Learners get multiple live learning paths computed from *transitive* prerequisite relationships against measured mastery. Set a goal concept; the system works backward through everything required to reach it.

> **Speaker notes:** Mention that (1) and (2) are separately licensable — a publisher may want only the generation engine; a university may want only the delivery framework. That optionality is deliberate in the patent structure, and for an angel it means more than one way the asset pays off.

---

## Slide 4 — Founder: I Designed This System in 1985

**Headline:** My master's thesis described Qlaudia. It failed for exactly one reason — and that reason no longer exists.

**[VISUAL: photograph of the 1985 thesis abstract page, beside the Qlaudia concept-graph screen]**

**1985 — the Conceptual Knowledge System (CKS)**, master's thesis, University of Kansas. A knowledge graph, built once and then used for two things:

> *"…the program has two intended functions: as an interactive knowledge acquisition facility and, secondly, as an information retrieval facility."*

**Acquisition and delivery, over a constructed graph.** Those are Qlaudia's two inventions, and the patent's two claim sets.

**How acquisition worked:**

> *"While engaged in interactive dialog with a user, CKS's acquisition facility attempts to acquire the concepts which constitute the user's knowledge."*

Every concept had to be extracted from a human being, one at a time. **The graph was never the hard part. Filling it was.**

**2026 — LLMs are the acquisition facility.** Same architecture. The missing half arrived.

> **Speaker notes:**
> **The structural point to make out loud.** CKS's two functions — acquisition and retrieval over a constructed knowledge graph — are the same two things Qlaudia does, and the same two things the patent claims separately. Forty-one years apart, the architecture decomposes identically. That is not a coincidence you have to sell; just show it and let them see it.
>
> **Say aloud, not on the slide — what else CKS got right:** retrieval worked by "the top down examination of an appropriately encoded set of concepts according to the logical relations that exist between the concepts" — prerequisite-ordered graph traversal. And it was proposed explicitly as an alternative to printed media, arguing that written prose "imposes unnecessary constraints on the organization of a body of knowledge." Full quotations in Appendix A6.
>
> **Do not claim conceptual primitives.** CKS also rested on a small set of conceptual primitives from which all concepts were defined. Qlaudia has no such basis and does not need one — see Appendix A6. Leave it out of the pitch entirely; it invites a question you'd have to answer with "that part isn't built."
>
> **This is the strongest slide in the deck. Consider opening the meeting with it, before the market slide.** A founder holding a 41-year-old thesis that describes the product he's now shipping is something no other pitch that month can imitate. It converts the entire "why you / why now / why hasn't this been done" cluster into a single artifact.
>
> **Bring the physical thesis to the meeting.** Angels invest in conviction and this is conviction you can hand across a table. The photograph on the slide is the fallback; the bound copy is the moment.
>
> **The move that makes it land is quoting your own limitation.** Don't present 1985 as a triumph — present it as a diagnosis. "I built this. It worked, structurally. It failed on acquisition, and I wrote that failure into my own abstract. That specific failure is what got solved in the last three years, and I recognized it the week it happened." Self-critical framing reads as far more credible than visionary framing, and the punchline hits harder.
>
> **Supporting career arc — say briefly, don't slide it:** expert systems at Boeing (1985), Lockheed Martin (1986–89), and Nortel (1989–93); then Cadence (finite state machine module shipped into multiple CAD products), Sprint (16 years, applications architect), DST Systems and TreviPay (workflow automation — dependency-graph execution, computing what can run given what's complete, which is transitive prerequisite pathfinding in different clothes). Then Charles Irvine Enterprises LLC and Academy-courses.com from 2017 — all predating the current AI cycle.
>
> **The 2017 date still matters.** Angels assume every AI-education pitch was conceived the week ChatGPT shipped. Between a 1985 thesis and a 2017 LLC, you can prove a four-decade throughline. That is the opposite of trend-chasing.
>
> **Anticipated question — "have you run a venture-backed company before?"** No. Don't dance. The true answer that lands: a working end-to-end pipeline and a filed non-provisional patent, built solo. Execution evidence is rarer at this stage than a prior exit.
>
> **The age question, which nobody will ask out loud.** This slide makes a 1985 start date unavoidable, and some angels carry an unspoken bias. The counter is the slide's own argument: you are not guessing about which AI paradigm is different, because you worked the previous one and documented precisely why it failed. Depth is the asset. Have a crisp, unbothered answer ready on energy and commitment, and don't let it sound defensive.
>
> **Institution — resolved, no action needed.** The thesis is University of Kansas, consistent with LinkedIn. Dr. van de Liefvoort, named on the thesis committee, is today emeritus at UMKC but did not join UMKC until August 1987 — two years after the thesis. If anyone ever cross-references him and raises it, that's the one-sentence answer.
>
> ⚠️ TODO: get a clean, straight scan of the abstract page and of the §1.3 "Approach and Scope" page — the phone photos won't hold up projected.
>
> ⚠️ TODO: advisors, collaborators, or committed early hires — still the one real gap. A solo founder with a named technical advisor reads materially safer to an angel than a solo founder alone.

---

## Slide 5 — Product

**Headline:** ⚠️ TODO — it already works. Show it.

- Create a domain live — the pipeline streams its progress on screen
- Browse the result: concept list, generated instruction, computed figures, assessments
- Knowledge graph visualization
- Progress and mastery tracking

> **Speaker notes:**
> For angels this is the highest-conviction slide in the deck, because it converts "interesting idea" into "this exists." Generating a domain *live on stage* is worth more than any slide you could put here.
>
> ⚠️ TODO: time a full generation run. If it's longer than ~90 seconds, pre-record it and play the recording — a live run that stalls in front of angels does more damage than a video.
>
> ⚠️ TODO: screenshots needed regardless, as fallback and for the send-after version of the deck.

---

## Slide 6 — Why the Content Can Be Trusted

**Headline:** The hard part isn't generating content. It's generating content that's *right*.

- **A concept graph, not a pile of documents** — every concept is a node, with prerequisite edges the system can reason over
- **Figures are computed and verified, not decorative** — diagrams are produced by executing generated construction code in a sandbox, checked against independently derived assertions, and automatically repaired on failure
- **The grader isn't the author** — assessment generation and figure verification run on a separate model from content generation
- **Structural importance ranking** — the system knows which concepts matter most by their position in the graph

> **Speaker notes:**
> Keep this slide short and non-technical out loud. The one line that lands with a non-technical angel: *"When Qlaudia draws a diagram, it doesn't sketch what a diagram usually looks like — it computes the actual figure and then checks it."* That's the difference between "AI wrote a textbook" and "AI wrote a textbook you'd let a student rely on."
>
> Full technical detail is in Appendix A2 for anyone who asks — don't preempt it on the slide.
>
> ⚠️ TODO: pull one genuinely impressive generated figure from a live domain as the visual. One good figure does this slide's whole job.

---

## Slide 7 — Why Now

**Headline:** Three curves crossed in the last 24 months.

- **Model capability** — frontier models can now hold a full subject's structure coherently, not just answer local questions
- **Inference cost** — generating a full domain has fallen from prohibitive to routine, and keeps falling
- **Institutional readiness** — post-2020, schools, universities, and employers have both the infrastructure and the permission to adopt digital-first learning

> **Speaker notes:**
> **Call straight back to Slide 4.** This slide is far more persuasive as "I documented the blocking constraint in 1985 and it was lifted in 2023" than as three generic market curves. The 1985 system had rigorous structure and no affordable acquisition. Today's chatbots have fluent acquisition and no structure. Qlaudia is the first moment both halves exist at once — and you can prove you've been holding one of them for forty years.
>
> ⚠️ TODO — add the actual per-domain generation cost. That single number *is* the why-now argument compressed, and it's likely startling enough to be the most memorable figure in the deck. "It costs $X to generate what CKS needed a human expert to type in one concept at a time" is the line angels repeat to each other afterward.

---

## Slide 8 — Defensibility

**Headline:** A filed patent, plus a content asset that compounds.

- **Non-provisional patent application filed** — App. No. 19/756,145, filed 2026-07-28
- **Two independent claim sets** — generation and delivery can be enforced and licensed separately
- **An accumulating graph** — every generated domain adds to a reusable, cross-linked corpus; shared concepts and prerequisites compound across subjects
- **Non-obvious engineering** — the verified-figure and QA architecture is substantial work that isn't visible from the outside

> **Speaker notes:**
> Say "filed, not granted" before anyone asks. Angels are less patent-sophisticated than VCs on average, which cuts both ways: some over-value a filing, and the ones who know better will test whether you're overselling it. Being precise unprompted wins both rooms.
>
> ⚠️ TODO: settle the exact wording if asked about the outstanding IDS and inventor declaration.

---

## Slide 9 — Business Model & First Customers

**Headline:** ⚠️ TODO — one primary motion, named, priced.

**The bottom-up number this slide must produce:**

> beachhead segment × realistic price × achievable penetration = **$⚠️ TODO**

### Beachhead

> **Upper-level math and science for homeschool families.**

### Why this segment first

- **No procurement** — parents decide in an evening and pay by card. No district sales cycle a solo founder can't survive.
- **The pain starts exactly where the parent's competence ends** — they can teach reading and arithmetic, not algebra II or chemistry. They already pay tutors for precisely this.
- **Their stated anxiety is prerequisite gaps** — *"is my kid actually ready for algebra II?"* That is literally what the prerequisite graph computes.
- **Verified figures matter most in math and science** — where our differentiator and their need coincide, and where competitors' AI content is weakest.

### Expansion path

Co-ops and microschools as buying groups → broader subject coverage → domain experts publishing their own schools → institutional.

**Pricing motion:** B2C subscription, direct. *(Full segment inventory and the alternatives considered: Appendix A9.)*

> **Speaker notes:**
> **This is the most important unfinished slide after the founder slide, and it's the one that pays off Slide 1.** A deck that opens on $7.3T and never names a reachable number reads as unserious. A deck that opens on $7.3T and then says *"and here is the $40M segment I can win first, at this price, with these first ten customers"* reads as ambitious *and* grounded.
>
> Listing five revenue models reads as having none. Pick one.
>
> **Why homeschool math/science is the recommended beachhead — the reasoning, for when an angel challenges it:**
>
> 1. **No procurement.** A solo founder cannot survive a nine-month district sales cycle. Homeschool parents decide in an evening and pay by card. This alone eliminates K–12 institutional, community college, and university as *first* markets, however large they are.
> 2. **The pain is sharpest exactly where the parent's own competence ends.** Most homeschool parents can teach reading and arithmetic. They cannot teach algebra II, precalculus, chemistry, or physics — and they know it. That's where they already spend real money on tutors, Saxon, Apologia, Thinkwell, Derek Owens.
> 3. **Their stated anxiety is literally prerequisite gaps.** "Is my kid actually ready for algebra II? What did we miss?" Qlaudia's transitive prerequisite graph and readiness computation answer the exact question this buyer lies awake about. No other segment's core anxiety maps this cleanly onto the core technology.
> 4. **Breadth of generation is a real advantage here.** One family needs many subjects across many grade levels. Generating any domain on demand is worth more to them than to a buyer who needs one fixed curriculum.
> 5. **The verified-figure pipeline matters most in math and science.** That is where a wrong diagram is fatal and where competitors' AI content is weakest. Differentiator and need coincide.
> 6. **Reachable, concentrated communities.** State homeschool associations, conventions, co-ops, curriculum-review sites, large Facebook and Reddit groups. Cheap acquisition without a sales team.
>
> **Honest risks to have answers for:** (a) AI-generated content skepticism runs high among homeschool parents, especially religious ones — the figure-verification and separate-QA-model story is the answer, and it's why Slide 6 exists; (b) buying is seasonal, concentrated in spring and summer; (c) price sensitivity is real — this is a value-conscious buyer.
>
> **Why not the other three you raised:**
> - **Supplementary for traditional-school parents** is a larger market but a worse fit: the subject is fixed by the school, so breadth stops mattering, and you compete head-on with free Khan Academy and entrenched IXL. High CAC, crowded.
> - **GED prep** has motivated buyers and genuine prerequisite gaps, but it's one fixed curriculum — it under-uses the generation engine entirely — and the population is price-sensitive and often funded through workforce programs, which puts you back into institutional selling.
> - **Domain experts publishing schools** is the right *second* act, not the first. It's a two-sided marketplace with a chicken-and-egg problem, and solving supply and demand simultaneously is not a solo-founder move. It becomes powerful once there's demand to sell into — and it's how content scales past you.
>
> ⚠️ TODO: Charles to confirm the beachhead, set a price point, and name the realistic first ten customers.

---

## Slide 10 — Traction

**Headline:** ⚠️ TODO

- Domains generated to date
- Users, signups, engagement
- Any institutional conversations, pilots, or LOIs
- **Cost and time per generated domain** — the hard efficiency metric

> **Speaker notes:** If early-stage traction is thin, reframe honestly around what *has* been de-risked: working end-to-end pipeline, filed patent, generated domains in production. Angels fund pre-traction all the time; they do not fund founders who seem to be hiding the absence of it.

---

## Slide 11 — Use of Funds

**Headline:** ⚠️ TODO — what this round buys, and the milestone it reaches.

- ⚠️ TODO: allocation across engineering / content / GTM / runway
- ⚠️ TODO: months of runway
- ⚠️ TODO: the specific milestone that makes the *next* round (or profitability) achievable

> **Speaker notes:** Angels care less about a spend breakdown than about one thing: **what is measurably true after this money that isn't true today?** Name that milestone explicitly and tie every allocation line to it.

---

## Slide 12 — The Ask

**Headline:** ⚠️ TODO — $⚠️ raising on a ⚠️ TODO.

- **Raising:** ⚠️ TODO amount
- **Instrument:** ⚠️ TODO — SAFE (post-money cap) / convertible note / priced round
- **Valuation cap:** ⚠️ TODO
- **Minimum check:** ⚠️ TODO
- **Committed to date:** ⚠️ TODO — including any founder capital
- **Target close:** ⚠️ TODO date

> **Speaker notes:**
> **This slide is the biggest structural difference between an angel deck and a VC deck.** A VC deck says "raising a seed round" and negotiates terms over subsequent weeks. An angel is often deciding *in the room*, and can't decide without knowing the instrument, the cap, and the minimum check. Leaving terms off the slide forces every interested angel to ask — and some won't.
>
> Naming a minimum check also does quiet qualification work: it tells a $10K angel they're looking at a syndicate, not a solo allocation, without an awkward conversation.
>
> ⚠️ TODO: Charles — a standard post-money SAFE is the lowest-friction instrument for a round of this shape, but the cap is a real decision. Worth a conversation before the first meeting, since it's hard to revise downward once quoted.

---

## Slide 13 — How This Returns Capital

**Headline:** ⚠️ TODO — the realistic exit paths.

**Likely acquirer categories:**

- **Publishers** — Pearson, McGraw Hill, Cengage: they own content and are structurally threatened by generated content
- **Learning platforms** — Coursera, Udemy, Chegg, Duolingo
- **LMS incumbents** — Instructure/Canvas, Anthology/Blackboard
- **Enterprise learning** — LinkedIn Learning, Docebo, Cornerstone
- **Big tech education arms** — Google, Microsoft
- ⚠️ TODO: comparable transactions and multiples in this space

> **Speaker notes:**
> **This slide does not exist in a typical VC deck, and it must exist here.** A VC's returns come from portfolio construction and they'll model exits themselves. An angel is writing a personal check with no fund structure behind it and is asking, consciously or not, *"how does this become money again?"* Answering it unprompted is a mark of respect for their position.
>
> Don't overreach on numbers — naming plausible acquirer *categories* and why each is structurally motivated is more credible than a fabricated multiple.
>
> Note the publishers are simultaneously the Slide 1 competition and the most motivated acquirers. That's a strength; say so.

---

## Appendix — sent after the meeting, not presented

### A1 — Competition

Suggested 2×2 axes: **structured & verified ↔ unstructured**, and **content generated ↔ content licensed or hand-built**.

- **General AI assistants** (ChatGPT, Claude, Gemini) — fluent, unstructured, no mastery model, no curriculum
- **Incumbent EdTech / LMS** (Canvas, Blackboard, Coursera, Khan Academy) — delivery infrastructure over hand-built content
- **AI tutoring startups** — conversation layers over existing curricula
- **Publishers** (Pearson, McGraw Hill, Cengage) — own the content, but it's manually produced and static

> ⚠️ TODO: Charles to confirm which competitors actually come up in his conversations. Moved out of the main deck for angels — the named-competitor grid is a VC-diligence artifact, and the differentiation argument is already carried by Slides 2, 3, and 6. Bring it back into the main deck if a specific investor asks.

### A2 — Technical architecture

Generation pipeline stages: concept map → atomic documents → computed figures (sandboxed execution + independently derived assertions + repair loop) → assessments → typed concept edges → prerequisite edges → embeddings → graph population.

Delivery: readiness computed over transitive prerequisite closure against per-concept mastery; multiple concurrent learning paths; goal-directed backward pathfinding.

### A3 — Roadmap

- Template layer for figure generation — the agreed next major build
- ⚠️ TODO: remaining 12–18 month milestones, tied to the Slide 11 funding milestone

### A4 — Patent detail

Non-provisional App. No. 19/756,145, filed 2026-07-28. Claim Set 1 covers AI-driven knowledge base generation; Claim Set 2 covers transitive-prerequisite adaptive delivery. The two claim sets are independently enforceable and licensable.

### A5 — The 1985 thesis: architectural correspondence

Source material for Slide 4. Charles Irvine, *The Conceptual Knowledge System (CKS)*, master's thesis, University of Kansas, 1985. ⚠️ TODO: confirm exact month; scan in full.

| CKS (1985) | Qlaudia (2026) |
|---|---|
| **Two functions: an acquisition facility and a retrieval facility, over one constructed graph** | **Two inventions — KB generation and adaptive delivery — and the patent's two claim sets** |
| Knowledge base of concepts | `Concept` nodes in Neo4j |
| "Logical relations that exist between the concepts" | Typed relationship edges + prerequisite edges |
| Retrieval facility: "top down examination… according to the logical relations" | Graph traversal, prerequisite-ordered learning paths |
| Minsky frame formalism | Structured concept schema |
| **Acquisition facility: interactive dialog interrogating a human expert** | **LLM generation pipeline — the half that was missing** |
| Proposed as an alternative to printed media, which "imposes unnecessary constraints on the organization of a body of knowledge" | Concept graph rather than linear documents |
| **"A small set of conceptual primitives" — all concepts ultimately defined in terms of them** | **Not carried forward. Qlaudia has no primitive basis.** |

### A6 — The 1985 thesis: key quotations

**Verify against the original before use.**

**The two that carry Slide 4:**

- Abstract, *what the system was*: *"Specifically, the program has two intended functions: as an interactive knowledge acquisition facility and, secondly, as an information retrieval facility."*
- Abstract, *how acquisition worked*: *"While engaged in interactive dialog with a user, CKS's acquisition facility attempts to acquire the concepts which constitute the user's knowledge."*

**Supporting:**

- Abstract: *"The retrieval facility serves the complementary function of allowing the traversal of a knowledge base that has been encoded through interaction with CKS."*
- Abstract, on guidance: *"The knowledge base serves the guidance function by providing a set of patterns which enable the program to anticipate the organization of the incoming information."*
- p. iii: *"The acquisition facility does succeed in the top down acquisition of a set of concepts. The retrieval facility… allows the top down examination of an appropriately encoded set of concepts according to the logical relations that exist between the concepts."*
- §1.3: *"It is hypothesized that a system similar in principle to the one described would in many circumstances be superior to a strict written language representation of knowledge which imposes unnecessary constraints on the organization of a body of knowledge."*
- §1.2: *"…might the computer serve to enrich the life of the individual? The author believes in the viability of this prospect."*

**Accurate but do not put on a slide:**

- p. iii: *"The user interface in general is quite terse and requires a knowledge of system details which could not normally be assumed. The program uses untried methods and is still in an experimental state."* — a true statement of the limitation, but it reads as a UI complaint rather than as the acquisition ceiling, and an audience has to be told what it means. Show the mechanism quote instead and let them infer it.

**On conceptual primitives.** CKS also held that all encoded concepts must ultimately be defined in terms of a small set of conceptual primitives (*"…another which consists of a small set of conceptual primitives"*). Kept here for the record only — see the warning below. It is not Qlaudia's architecture and should stay out of the pitch.

> **Note on the last quotation.** It is the mission statement of this company, written in 1985. If there is a closing line for the whole pitch, it may be that sentence — read aloud from the original, then: *"I still believe it. Now it's buildable."* Use once, at the end, and don't explain it afterward.

**The primitives idea is NOT in Qlaudia — do not claim otherwise.** CKS rested on a closed basis: a small set of conceptual primitives in terms of which every encoded concept had ultimately to be defined. Qlaudia does the opposite. `step4_edges.py` has the LLM generate a fresh, domain-specific relationship vocabulary per subject, explicitly preferring specificity (`TRANSFERS_POWER_TO`, not `RELATED_TO`). The only closed set in the system is a six-value `archetype` tag — functional, hierarchical, causal, spatial, temporal, safety — which *classifies* relations rather than serving as a basis from which concepts are composed.

The Substance/Relation/Change/Extent framework in `patent_application/The_Four_Emergent_Realities.md` is a separate philosophical document. It is **not implemented**. Treat it as a research direction, never as a shipped capability — an overclaim here is the kind an even mildly technical investor can disprove by reading the schema, and it would put every other claim in the deck in question.

**On the thesis committee.** Dr. Appie van de Liefvoort moved to UMKC in August 1987 and is emeritus there now. Noted only because a diligence search on his name surfaces UMKC and could look like a mismatch with the University of Kansas — the dates rule it out.

### A7 — Market sources

- HolonIQ, *$10 Trillion Global Education Market in 2030* — https://www.holoniq.com/notes/10-trillion-global-education-market-in-2030
- HolonIQ, *Global EdTech market to reach $404B by 2025* — https://www.holoniq.com/notes/global-education-technology-market-to-reach-404b-by-2025
- HolonIQ, *The Size & Shape of the Global Education Market* — https://www.holoniq.com/notes/the-size-shape-of-the-global-education-market
- U.S. Census Bureau, *Public School Spending Per Pupil Reaches Historic High in 2024* — https://www.census.gov/newsroom/press-releases/2026/school-system-finances.html
- EdChoice, *How Much Do Public Schools Spend?* — https://www.edchoice.org/2026-how-much-do-public-schools-spend/
- NCES, *Fast Facts: Expenditures* — https://nces.ed.gov/fastfacts/display.asp?id=66
- Statista, *Expenditure of public and private colleges and universities* — https://www.statista.com/statistics/184231/expenditure-of-public-and-private-colleges-and-universities
- Grand View Research, *Corporate Training Market Report* — https://www.grandviewresearch.com/industry-analysis/corporate-training-market-report
- Fortune Business Insights, *Private Tutoring Market* — https://www.fortunebusinessinsights.com/private-tutoring-market-104753
- Mordor Intelligence, *Language Learning Market* — https://www.mordorintelligence.com/industry-reports/language-learning-market

**Cross-sector comparison and capital gap (Slide 1):**

- WHO, *Global spending on health* (2024 report, data through 2022; $9.8T, 9.9% of global GDP) — https://www.who.int/teams/health-financing-and-economics/global-spending-on-health-report
- Gartner, *Worldwide IT Spending Forecast* ($5.43T, 2025) — https://www.gartner.com/en/newsroom/press-releases/2025-07-15-gartner-forecasts-worldwide-it-spending-to-grow-7-point-9-percent-in-2025
- SIPRI, *Trends in World Military Expenditure, 2024* ($2.718T) — https://www.sipri.org/publications/2025/sipri-fact-sheets/trends-world-military-expenditure-2024
- HolonIQ, *EdTech VC reached ~$2.4B for 2024, the lowest level of investment in a decade* — https://www.holoniq.com/notes/edtech-vc-reached-2-4b-for-2024-representing-the-lowest-level-of-investment-in-a-decade
- HolonIQ, *EdTech funding drops again in early 2025* — https://www.holoniq.com/notes/edtech-funding-drops-again-in-early-2025-fewer-deals-but-bigger-bets
- EdWeek Market Brief, *2024 Was the Worst Year for Ed-Tech VC Funding in a Decade* — https://marketbrief.edweek.org/financing-investment/2024-was-the-worst-year-for-ed-tech-vc-funding-in-a-decade-this-year-looks-even-worse/2025/05

**Caveat for diligence:** segment figures come from commercial market-research firms whose estimates vary widely by methodology (private tutoring alone is reported anywhere from ~$67B to ~$134B for 2025). The HolonIQ top-line and the U.S. government figures are the two most defensible numbers on Slide 1; lead with those and treat the rest as directional.

### A8 — The same market, viewed from the United States

Moved off Slide 1 to keep it presentable. Use if an American angel asks for domestic figures.

| Segment | Annual spend |
|---|---|
| U.S. K–12 public schools | **~$1.0T** (FY2024, first year over $1T; ~$17.6K per pupil) |
| U.S. higher education institutions | **~$712B** total institutional expenditure |
| U.S. corporate & workplace training | ~$100B |
| U.S. private tutoring | ~$30B and growing double digits |

### A9 — Full candidate segment inventory

Working material behind Slide 9. **Direct-pay parents and learners — no procurement cycle:**

- **Homeschool families** — buy curriculum directly, need many subjects across many grade levels
- **Homeschool co-ops & microschools** — same buyer, multi-seat, higher ACV
- **Supplementary learning for traditional-school parents** — math and science alongside school
- **GED preparation** — adult learners with genuine, diagnosable prerequisite gaps
- **Gifted / accelerated learners** — need to move fast through prerequisites, not slowly
- **Test prep** — SAT/ACT, GRE, MCAT, LSAT
- **Adult career changers** — self-funded, outcome-motivated

**Credential-driven buyers — clear outcome, high willingness to pay:**

- **Professional licensure** — CPA, bar, NCLEX/nursing, PE, actuarial, real estate, insurance
- **IT & cloud certification** — AWS, Azure, CompTIA, Cisco, security
- **Trades & vocational** — HVAC, electrical, welding
- **Continuing education** — CME, CLE, CPE

**Supply-side / platform:**

- **Domain experts publishing their own schools** — the expert brings expertise, Qlaudia does the production. `School` nodes and per-school course listings already exist in the data model
- **Tutoring companies** — sell them the curriculum engine rather than compete with them
- **Publishers & platforms** — generation-engine API licensing

**Institutional — long cycles, deliberately deferred:**

- K–12 districts · community college developmental ed · university gateway-course remediation · corporate L&D on proprietary internal domains · special education, where prerequisite structure *is* the pedagogical requirement

**Alternative pricing motions:** B2B2C institutional licensing · enterprise training seats · generation-engine API licensing · marketplace revenue share on expert-published schools · patent licensing of either invention independently.

**Why not the three alternatives most often raised:**

- **Supplementary for traditional-school parents** — larger, but the subject is fixed by the school so breadth stops mattering, and it competes head-on with free Khan Academy and entrenched IXL. High CAC, crowded.
- **GED prep** — motivated buyers and real prerequisite gaps, but one fixed curriculum under-uses the generation engine, and the population is price-sensitive and often workforce-funded, which returns you to institutional selling.
- **Domain experts publishing schools** — the right second act. A two-sided marketplace needs supply and demand solved simultaneously, which is not a solo-founder first move. It becomes powerful once there is demand to sell into, and it is how content scales past the founder.
