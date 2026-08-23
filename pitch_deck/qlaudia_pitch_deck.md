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

## Slide 2 — Education Is the Largest Untransformed Market on Earth

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

- **Corporate training** — ~$427B global
- **Private tutoring** — ~$134B global
- **Language learning** — ~$85B global
- **Test prep & admissions** — SAT, ACT, GRE, MCAT, LSAT
- **Professional licensure & continuing education** — CME, CLE, CPE, bar, nursing, trades
- **IT & technical certification** — AWS, Azure, Cisco, CompTIA
- **Homeschooling, microschools & pods**
- **Compliance & regulatory training**
- **Military, government & NGO training**
- **Self-directed learning, bootcamps & courseware publishing**

> **Speaker notes:**
> **U.S. figures, if an American angel wants them (full table in Appendix A8):** K–12 public schools ~$1.0T in FY2024, the first year over a trillion, ~$17.6K per pupil. Higher education ~$712B. Corporate training ~$100B. Private tutoring ~$30B and growing double digits.
>
> Say out loud, before anyone else says it: *"No company captures a market this size, and I'm not going to pretend otherwise."* Saying it first converts the deck's biggest liability into a credibility marker. Then land the actual point, which is **structural, not arithmetic**: education is the last enormous market where the core product — a coherent, sequenced body of knowledge taught in the right order — has never been *manufacturable*. It's hand-built by humans, one course at a time. That's why it costs what it costs. Qlaudia makes the knowledge itself manufacturable.
>
> Then immediately promise the follow-through: *"the Business Model slide shows the specific slice I'm going after first, and what it's worth."* An angel who hears a $7.3T number and never hears a reachable number assumes you can't tell the difference. Don't leave that gap open across eight slides.
>
> Anticipated pushback: *"EdTech is a graveyard."* Correct — because prior EdTech sold *delivery* (an LMS, a video player, a quiz engine) into institutions that already had content. Qlaudia sells the content layer itself, which is the expensive part.
>
> **The capital-gap stat — hold this in reserve, do not volunteer it.** Digital health VC is on track for ~$28B in 2025. EdTech VC was ~$2.4B in 2024, a decade low, and Q1 2025 fell another 35%. Normalized against sector size, healthcare draws roughly **9× more venture capital per dollar of sector spending** than education does — a market three-quarters the size of healthcare attracting one-twelfth the venture dollars.
>
> This stat cuts both ways and the framing decides which. Volunteered cold it reads as *"the market has spoken and it said no."* Deployed as the answer to "isn't EdTech a graveyard?" it is devastating: *"Yes — and that's why I can build a healthcare-scale company with no competition for capital or talent. The graveyard is full of companies that sold delivery. I sell the content."* Say it only after you've named why the prior generation failed.
>
> **Year alignment — be precise if pressed.** WHO's latest global health figure is 2022 ($9.8T); healthcare today is likely ~$11T. Against a 2025 education number, the honest ratio is closer to two-thirds than three-quarters. The years are labelled on the slide for exactly this reason — don't let a sharp angel be the one to point it out.

---

## Slide 3 — The Three Numbers That Matter

**Headline:** The market is enormous, almost entirely analog, and nobody is selling the thing that would change that.

1. **~$7.3T** — spent teaching people every year, growing to **$10T by 2030**
2. **~5%** — of it is digital. The rest is people, buildings, and paper
3. **$0** — goes to a system that can generate a verified, prerequisite-structured course on demand

> **Speaker notes:**
> **Split off the Market slide deliberately — these three numbers are the argument, and they were getting buried under two tables.** Delivered on their own slide they land as a sequence: enormous, analog, unserved. Pause after each.
>
> Number three is the one that does the work. One and two are context an informed angel may already half-know; three is the claim only you can make, and it sets up every slide that follows.
>
> If you are running short on time, this is the slide to linger on and the Market slide is the one to move through quickly — the tables are reference material, this is the thesis.

---

## Slide 4 — The Problem

**Headline:** Every course is written from scratch by one expert. That's why education doesn't scale, doesn't adapt, and doesn't transfer.

- **Content is hand-built.** A single university course takes an expert months. A curriculum takes years. Cost scales linearly with subjects covered.
- **Structure is implicit.** Prerequisites live in a professor's head or a syllabus footnote — not in a machine-readable form anything can reason over.
- **Sequencing is one-size-fits-all.** Everyone walks the same path at the same pace regardless of what they already know.
- **AI chatbots don't fix this.** An LLM answers any question fluently, but it has no model of *what you know*, *what you must learn first*, or *whether the explanation it just gave was correct*. It tutors without a curriculum.
- **And it re-derives the same lesson for every learner.** A chatbot regenerates algebra from scratch for each student, each time — unverified, slightly different, and paid for again on every ask.

> **Speaker notes:**
> The chatbot bullet is the one that matters. Every angel in the room has already used ChatGPT to learn something and has a private opinion about how well it went. Make the distinction concrete: a chatbot is a conversation that evaporates; Qlaudia is a structured, persistent, verifiable body of knowledge that a conversation can stand on.
>
> **Optional setup for the Founder slide.** If you want the founder slide to detonate, plant the fuse here: "the hand-authoring bottleneck isn't new — it's the reason this whole approach stayed impractical for forty years." Then let the Founder slide reveal that you were one of the people who hit that wall and wrote it down.

---

## Slide 5 — The Solution

**Headline:** Qlaudia generates a complete, prerequisite-structured knowledge graph for any subject — in hours, not months — and teaches from it adaptively.

**Two inventions, independently valuable:**

1. **Knowledge base generation.** Point Qlaudia at a subject. It produces a graph of concepts, each with written instruction, computed figures, worked examples, and assessments — plus the typed relationships and prerequisite edges that connect them.
2. **Adaptive, goal-directed delivery.** Learners get multiple live learning paths computed from *transitive* prerequisite relationships against measured mastery. Set a goal concept; the system works backward through everything required to reach it.

> **Speaker notes:** Mention that (1) and (2) are separately licensable — a publisher may want only the generation engine; a university may want only the delivery framework. That optionality is deliberate in the patent structure, and for an angel it means more than one way the asset pays off.
>
> **Set up the demo here.** "Any subject" is the strongest claim on this slide and the hardest to believe. Promise the evidence rather than arguing for it: *"In two slides I'll show you it building a course on raising an angel round."* Then stop — let them sit with the claim knowing proof is coming.

---

## Slide 6 — Founder: I Designed This System in 1985

**Headline:** My master's thesis described Qlaudia. I earned my master's degree in CS. But the ideas could not have been put into practice — until now.

**1985 — the Conceptual Knowledge System (CKS)**, master's thesis, University of Kansas. A knowledge graph, built once and then used for two things:

> *"…the program has two intended functions: as an interactive knowledge acquisition facility and, secondly, as an information retrieval facility."*

**Acquisition and delivery, over a constructed graph.** Those are Qlaudia's two inventions, and the patent's two claim sets.

**How acquisition worked — and why it wasn't practical:**

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
> **Bring the physical thesis to the meeting.** Angels invest in conviction and this is conviction you can hand across a table. With no image on the slide, the bound copy is now the *only* visual — so don't leave it at home.
>
> **Be precise: CKS did not fail.** The thesis was accepted and it earned the MS. The system worked — it acquired concepts, encoded them, and traversed them. What it wasn't was *practical*: filling the knowledge base required interrogating a human expert one concept at a time, so the cost of a useful knowledge base was prohibitive. Never say "it failed" — it's inaccurate, it implies the thesis was rejected, and it's a weaker claim than the true one.
>
> **The move that makes it land is naming the constraint in your own words.** Don't present 1985 as a triumph *or* as a failure — present it as a correct design waiting on an input that didn't exist yet. "I built this. It worked. It was never practical, because every concept had to come out of a human being one at a time. That constraint is what lifted in the last three years, and I recognized it the week it happened." Naming your own blocking constraint reads as far more credible than visionary framing, and the punchline hits harder.
>
> **Supporting career arc — say briefly, don't slide it:** expert systems at Boeing (1985), Lockheed Martin (1986–89), and Nortel (1989–93); then Cadence (finite state machine module shipped into multiple CAD products), Sprint (16 years, applications architect), DST Systems and TreviPay (workflow automation — dependency-graph execution, computing what can run given what's complete, which is transitive prerequisite pathfinding in different clothes). Then Charles Irvine Enterprises LLC and Academy-courses.com from 2017 — all predating the current AI cycle.
>
> **The 2017 date still matters.** Angels assume every AI-education pitch was conceived the week ChatGPT shipped. Between a 1985 thesis and a 2017 LLC, you can prove a four-decade throughline. That is the opposite of trend-chasing.
>
> **Anticipated question — "have you run a venture-backed company before?"** No. Don't dance. The true answer that lands: a working end-to-end pipeline and a filed non-provisional patent, built solo. Execution evidence is rarer at this stage than a prior exit.
>
> **The age question, which nobody will ask out loud.** This slide makes a 1985 start date unavoidable, and some angels carry an unspoken bias. The counter is the slide's own argument: you are not guessing about which AI paradigm is different, because you worked the previous one and documented precisely what it was missing. Depth is the asset. Have a crisp, unbothered answer ready on energy and commitment, and don't let it sound defensive.
>
> **Institution — resolved, no action needed.** The thesis is University of Kansas, consistent with LinkedIn. Dr. van de Liefvoort, named on the thesis committee, is today emeritus at UMKC but did not join UMKC until August 1987 — two years after the thesis. If anyone ever cross-references him and raises it, that's the one-sentence answer.
>
> ⚠️ TODO: get a clean, straight scan of the abstract page and of the §1.3 "Approach and Scope" page — the phone photos won't hold up projected.
>
> ⚠️ TODO: advisors, collaborators, or committed early hires — still the one real gap. A solo founder with a named advisor reads materially safer to an angel than a solo founder alone.
>
> **The efficient way to close it:** a recognised homeschool community figure — a co-op director, a curriculum reviewer, a well-followed practitioner — taken on as an advisor with a small vesting equity grant. That fills the credibility gap on this slide *and* creates a committed distribution partner (Appendix A11) with the same person. One conversation solves two of the deck's open problems.

---

## Slide 7 — Watch It Build a Course

**Headline:** Here is Qlaudia building a complete course on raising an angel round — the one subject in the world you can grade on sight.

**[VIDEO: recorded end-to-end run, time-lapsed to ~90 seconds]**

- **The ask** — a plain-language description of the course you want. That is the entire input
- **The advisor** — the model interrogates that description and turns it into a structured brief: audience, coverage, outcome, tone
- **The syllabus** — proposed concepts, reviewed and edited by the author *before* a word is written
- **The pipeline** — instruction, computed figures, assessments, typed relationships, prerequisite graph
- **The finished course** — and the prerequisite graph showing what must be understood before what

**A paragraph in. A complete course out, in about 18 minutes, unattended.**

> **Speaker notes:**
> **Say it is a recording, in the first sentence.** *"This is recorded — I'm not going to make you watch eighteen minutes."* If they suspect staging you lose more than the demo gains, and the honesty costs nothing. A live run is not worth the risk: eighteen minutes of runtime, a network dependency, and a known truncation bug are three ways to fail in front of the people you are asking for money.
>
> **Why this subject, said out loud:** *"I picked the one subject everyone in this room already knows cold, so you can judge the output instead of taking my word for it."* That is the whole point — on any other topic they would have to trust you.
>
> **Start the recording at the input screen, not at the pipeline.** The opening seconds carry the argument: what goes in is a paragraph a person could write in two minutes. Everything after that is machine. If you start mid-pipeline, the audience never learns how little was required, and the effort asymmetry is the point of the whole slide.
>
> **Name the two human checkpoints — they are features, not overhead.** The advisor interrogating the description shows the system pushes back on a vague ask rather than generating regardless. The syllabus review shows the author approves the concept list *before* any content is produced. For an angel whose instinctive worry is "AI slop," the visible answer is that a person signs off on the outline and the machine does the labour. Do not let these read as loading screens; say what each one is as it appears.
>
> **The callback to the Founder slide, if you want it.** CKS also worked by interrogating a human — but it interrogated them for the *knowledge*, one concept at a time, which is what made it impractical. Qlaudia's advisor interrogates you for your *intent*, which takes two minutes, and the model supplies the knowledge. The dialogue survived; what it asks for is what changed. This is a good line and easy to overplay — use it once, in one sentence, and move on.
>
> **The offer that replaces the live demo — make it before you leave.** A recording can be cherry-picked and sophisticated investors know it, so recover the proof afterward: *"Name any subject. I'll send you the course tomorrow."* Zero risk, more impressive than a live run, and it turns the demo into a reason to talk again — which is exactly what you want from an angel who has not committed.
>
> **⚠️ TODO — read the course before you record it.** Pre-generating exists precisely so you can inspect before they do; skipping that step throws away the main advantage of not going live. You do not need to review everything: read the 5–8 concepts that appear on camera, plus anything touching deal terms, dilution, or valuation caps. Roughly twenty minutes. Fix or cut what is wrong — you control the edit.
>
> Two reasons this matters more here than it would on any other topic: an angel needs one glance at one paragraph to catch an error about angel investing, and a visible mistake does not read as a typo — it contradicts the Pipeline slide's claim of a verified pipeline. A clean demo gains you a little; a caught error costs you a lot.
>
> **Remember they will look again later.** The plan is to hand them the course link. In the room nobody inspects. Alone that evening, with time, they will.
>
> ⚠️ TODO: record end to end — from typing the description, through the advisor exchange and the syllabus review, to browsing the finished course. Time-lapse the long stretches; keep the input and the review at real speed, since those are the parts that carry meaning. Keep the raw capture too — the unedited pipeline log is good diligence material.
>
> ⚠️ TODO: still screenshots as a fallback for a room with no video, and for the send-after version of the deck.

---

## Slide 8 — This Is a Pipeline, Not a Prompt

**Headline:** Producing a course that is correct, structured, and reusable is hard engineering. This is the machine that does it.

- **Mined once, then served** — knowledge is distilled into a durable graph up front, not re-derived on every question. We pay for inference once per concept, not once per learner
- **Figures are computed, executed, and checked** — diagrams come from generated construction code run in a sandbox, verified against independently derived assertions, and automatically repaired on failure
- **The grader isn't the author** — assessments and figure verification run on a separate model from the one that wrote the content
- **A concept graph, not a pile of documents** — typed relationships and prerequisite edges the system computes over
- **Structural importance ranking** — graph centrality identifies which concepts carry the most weight

> **Eight pipeline stages. Two models. A sandbox. A repair loop.**

> **Speaker notes:**
> **The job of this slide is to answer "isn't this just a wrapper?" before anyone asks it.** By this point they've seen the claim (the Solution slide) and the product (the Demo slide). The live question is not whether the content is trustworthy — it's whether there is anything here a competent engineer couldn't rebuild in a weekend with a good prompt. Answer that by showing the machinery. Trust is the conclusion they draw on their own; do not ask for it, and do not frame this slide as a defense of quality.
>
> Keep it short and non-technical out loud. The one line that lands with a non-technical angel: *"When Qlaudia draws a diagram, it doesn't sketch what a diagram usually looks like — it computes the actual figure and then checks it."* That's the difference between "AI wrote a textbook" and "AI wrote a textbook you'd let a student rely on."
>
> **Mine-once is the architectural keystone — say it first, because everything else depends on it.** You cannot verify an explanation that doesn't exist yet. The figure pipeline runs generated construction code, checks it against assertions, and repairs it on failure — a loop that takes far too long to run inside a live chat turn. Doing the work once, offline, with a repair budget, is what makes verification affordable at all. A chatbot can't do this not because the model is weaker, but because the architecture forecloses it.
>
> **Point back at the demo — they just watched this list happen.** Every bullet here was visible on the previous slide: the pipeline stages, the figure repair loop retrying, the QA model running separately. This slide is the narration for footage they have already seen, which is far stronger than describing machinery in the abstract. If you cut anything for time, cut the words, not the video.
>
> **Where content quality does belong: as a commercial advantage, not a disclaimer.** Homeschool parents (the beachhead on the Business Model slide) are genuinely skeptical of AI-generated material, and verified figures are how you win that objection *in the market*. Deploy it there — in a sales conversation, or when an angel raises it — rather than pre-empting a doubt half the room didn't have.
>
> **Three more consequences worth having ready:**
> - **Errors get fixed permanently.** A stored concept is corrected once and every future learner gets the correction. A chatbot's mistake recurs indefinitely, because there's no artifact to fix.
> - **Every learner gets the same vetted explanation.** Re-derivation means each student receives a slightly different, individually unverified lesson.
> - **You can compute over a graph that exists.** Importance ranking and prerequisite pathfinding are algorithms over a persisted structure — there is nothing to run them on if the content is generated per question.
>
> **The margin version — this is the one that matters to an investor.** Most AI startups are inference pass-throughs: cost of goods scales linearly with usage, so gross margin never improves and the model provider captures the upside. Qlaudia inverts that. Generation cost is incurred **once per concept and amortized across every learner who ever studies it**, so cost per learner falls toward zero as usage grows. The asset appreciates while COGS stays flat. If an angel asks "isn't this just a wrapper?" — this is the answer, and it's a structural one, not a claim about the product.
>
> Full technical detail is in Appendix A2 for anyone who asks — don't preempt it on the slide.
>
> ⚠️ TODO: pull one genuinely impressive generated figure from a live domain as the visual. One good figure does this slide's whole job.

---

## Slide 9 — Why Now

**Headline:** Three curves crossed in the last 24 months.

- **Model capability** — frontier models can now hold a full subject's structure coherently, not just answer local questions
- **Inference cost** — generating a complete course now costs **roughly $5** in model calls. A subject-matter expert writing the same thing takes months
- **Institutional readiness** — post-2020, schools, universities, and employers have both the infrastructure and the permission to adopt digital-first learning

> **~$5 and about 15 minutes** to generate a ~34-concept course with written instruction, computed figures, ~107 assessment questions, and a full prerequisite graph.

> **Speaker notes:**
> **Call straight back to the Founder slide.** This slide is far more persuasive as "I named the blocking constraint in 1985 and it was lifted in 2023" than as three generic market curves. The 1985 system had rigorous structure and no affordable acquisition. Today's chatbots have fluent acquisition and no structure. Qlaudia is the first moment both halves exist at once — and you can prove you've been holding one of them for forty years.
>
> **Attach the number to the course they just watched.** Not an abstract unit cost — *that* course, the one about raising an angel round: *"That cost about five dollars to produce."* A figure tied to an artifact in front of them is far harder to wave off than a figure on a slide.
>
> **The $5 figure is the most repeatable line in the deck.** "It costs about five dollars to generate what CKS needed a human expert to type in one concept at a time" is what angels say to each other afterward. Deliver it as a fact, not a boast, and let them do the multiplication.
>
> **⚠️ It is currently an ESTIMATE, not a measurement — say so if pressed.** It is derived bottom-up from the 64 domains already in the graph (concept counts, corpus size, edge counts) priced at current model rates; the full derivation is in Appendix A10. Cost instrumentation now runs on every generation, so this becomes a measured number on the next domain created. **Replace the estimate with the measured figure before the first investor meeting** — "we measured it" is a materially stronger answer than "we estimated it," and you're one pipeline run away from being able to say it.
>
> **If asked "how do you know?"** — the honest answer is strong: every stored domain's concept count, content volume, and edge count is known, and model pricing is public. The estimate is arithmetic over real artifacts, not a guess. Offer the appendix.
>
> **Do not quote a cost lower than ~$5.** Anthropic's Sonnet 5 introductory rate expires 2026-08-31; the $5 figure already assumes the higher post-promo rate, so it stays true after the promo lapses. A number that expires this month is the wrong number for a deck.

---

## Slide 10 — Defensibility

**Headline:** A filed patent, plus a content asset that compounds.

- **Non-provisional patent application filed** — App. No. 19/756,145, filed 2026-07-28
- **Two independent claim sets** — generation and delivery can be enforced and licensed separately
- **An appreciating asset** — the graph is generated once and served indefinitely. Every domain adds to a reusable, cross-linked corpus, and generation cost amortizes across every learner who ever uses it
- **Non-obvious engineering** — the verified-figure and QA architecture is substantial work that isn't visible from the outside

> **Speaker notes:**
> Say "filed, not granted" before anyone asks. Angels are less patent-sophisticated than VCs on average, which cuts both ways: some over-value a filing, and the ones who know better will test whether you're overselling it. Being precise unprompted wins both rooms.
>
> ⚠️ TODO: settle the exact wording if asked about the outstanding IDS and inventor declaration.

---

## Slide 11 — Business Model & First Customers

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

### How we reach them — creators, not ads

- **Homeschool creators publish their own schools.** A curriculum reviewer with 40,000 subscribers gets *"Mrs. Anderson's Chemistry"* under her own name, for her audience
- **Paid on revenue share**, not sponsorship — the channel costs nothing until it converts
- Then **co-ops and associations** as buying groups, and institutional last

**Pricing motion:** B2C subscription, direct. *(Full segment inventory: Appendix A9. Channel plan: Appendix A11.)*

> **Speaker notes:**
> **This is the most important unfinished slide after the founder slide, and it's the one that pays off the Market slide.** A deck that opens on $7.3T and never names a reachable number reads as unserious. A deck that opens on $7.3T and then says *"and here is the $40M segment I can win first, at this price, with these first ten customers"* reads as ambitious *and* grounded.
>
> Listing five revenue models reads as having none. Pick one.
>
> **Close the gap the demo just opened — one sentence, unprompted.** They watched you build a startup-finance course and are now hearing about homeschool math. Say it before they wonder: *"The demo was a proof of generality, not the market I'm entering."* Left unsaid, the obvious question is "so which business is this?", and an angel who thinks you are undecided about your market stops listening to the rest.
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
> **Honest risks to have answers for:** (a) AI-generated content skepticism runs high among homeschool parents, especially religious ones — the figure-verification and separate-QA-model story from the Pipeline slide is the answer, deployed here as a sales argument rather than a disclaimer; (b) buying is seasonal, concentrated in spring and summer; (c) price sensitivity is real — this is a value-conscious buyer.
>
> **Why not the other three you raised:**
> - **Supplementary for traditional-school parents** is a larger market but a worse fit: the subject is fixed by the school, so breadth stops mattering, and you compete head-on with free Khan Academy and entrenched IXL. High CAC, crowded.
> - **GED prep** has motivated buyers and genuine prerequisite gaps, but it's one fixed curriculum — it under-uses the generation engine entirely — and the population is price-sensitive and often funded through workforce programs, which puts you back into institutional selling.
> - **Domain experts publishing schools** is the right *second* act, not the first. It's a two-sided marketplace with a chicken-and-egg problem, and solving supply and demand simultaneously is not a solo-founder move. It becomes powerful once there's demand to sell into — and it's how content scales past you.
>
> ⚠️ TODO: Charles to confirm the beachhead, set a price point, and name the realistic first ten customers.

---

## Slide 12 — Traction

**Headline:** Live in production — 63 courses, and the first users are finishing them.

**Built** *(production graph, not projections)*

| | |
|---|---|
| Courses live | **63** across 7 schools |
| Concepts | **2,106** |
| Assessment questions | **6,755** |
| Prerequisite edges | **8,837** |
| Typed relationships | **13,523** |
| Generated instruction | **~3.9M tokens** |

**Used** *(early, and honest about it)*

- **One user completed five courses end to end** — 224 concepts, every one finished
- **Two more worked a course to 92%**
- 86 site visitors over the last four months; 15 accounts, 25 enrolments
- ⚠️ TODO: institutional conversations, pilots, or LOIs

> **Speaker notes:**
> **Lead with what's built, then volunteer what isn't.** The build numbers are real artifacts in the production graph — verifiable in a single query — produced by one person. That is execution evidence, and it is the strongest thing on the slide.
>
> **The single best data point you have is one person.** Five arrhythmia courses, 224 concepts, every one completed, in sequence. That is not browsing — that is someone using Qlaudia as their actual learning path through a hard clinical subject, and analytics show roughly 23 hours of engagement behind it. One user like that is worth more than a thousand visitors, and an angel knows it. Name him, describe what he did, and stop.
>
> **Say the quiz number before they find it.** Nobody in production has answered a single assessment question — competency is 0% across every user. Progress is self-marked "got it," not demonstrated mastery. Volunteer this: it is a product-surfacing problem, it is fixable, and it is exactly the kind of thing that destroys credibility if they discover it after you have described assessments as a differentiator on the Pipeline slide.
>
> **Be equally straight about the funnel.** 86 visitors produced 15 accounts, and most engaged sessions come from two locations — Charles and the one power user. The honest reading is that the product works on the people who reach it, and almost nobody reaches it. That is a conversion problem, not a proof problem, and it is what the round addresses.
>
> **The reframe that works:** the risk retired here is *technical*. The pipeline works end to end, the content is verifiable, the patent is filed, and real users complete real courses. What is unproven is distribution — which is exactly what this round buys.
>
> ⚠️ TODO: refresh these figures the week of the pitch; they move. `scripts/list_user_enrollments.py --prod` produces the usage half.

---

## Slide 13 — Use of Funds

**Headline:** The product is built. This round buys distribution — and the infrastructure to survive it.

**1 · Distribution — $⚠️ TODO**
Creator partnerships on revenue share, co-op and association relationships, and the conversion work the funnel needs.

**2 · Hardening — $⚠️ TODO**
Everything currently runs on free tiers. Managed Neo4j with backups, an always-on backend (no cold starts on an 18-minute pipeline), observability, and hard rate limits on course generation.

**3 · Operating runway — $⚠️ TODO**
Founder compensation, baseline hosting, and tooling through the build-up period.

> **Total: $⚠️ TODO — ⚠️ N months, carrying us through the spring 2027 buying cycle.**

> **What that buys:** ⚠️ TODO — *"By the spring 2027 cycle we have N creator partners, M paying families, and completion data."*

> **Speaker notes:**
> **Open with the asymmetry, in these words:** *"Most people at this stage are asking you to fund a build. I've already built it. This round funds getting it in front of people, and the infrastructure to handle them when they arrive."* Most angel deals carry both build risk and market risk; you are asking them to carry one. Say so — it is the single strongest framing available to you and it belongs here, not buried.
>
> **Say "feature-complete, hardening needed for scale," never "complete."** The product works, has never met load, and runs on free tiers. The precise version is credible and justifies line item 2; the simple version invites someone to go find the exception — and they will.
>
> **Rate limiting is a financial control, not a performance one.** Each generated course costs about $5 in model calls. Exposed without hard limits, that is a direct attack surface on your bank account. Saying this demonstrates you understand your own unit economics as a liability, not only as a selling point.
>
> **Why revenue starts when it starts — the calendar, not drift.** Homeschool curriculum is bought February through August; the 2026 cycle has closed. Pre-revenue here is externally imposed and dateable, which is a far better answer than any traffic projection: *"this round funds the run-up to a known buying window."*
>
> **Angels care about one thing on this slide: what is measurably true afterwards that isn't true today.** Name that milestone, then tie all three buckets to it.
>
> **The total on this slide must equal the raise on slide 14.** That is the whole reason the three buckets are stated in dollars rather than two in dollars and one in months — an angel should be able to add them up in their head and land on your ask. If the numbers don't reconcile, the obvious question is where the remainder goes, and it implies the round size was chosen before the plan. Decide what the work costs, sum it, and let that be the ask — never the reverse.
>
> ⚠️ TODO: the numbers. Three bucket amounts, the total, and the months of runway that total represents — the total drops straight into slide 14, so settle this slide first.

---

## Slide 14 — The Ask

**Headline:** ⚠️ TODO — $⚠️ raising on a ⚠️ TODO.

### The terms

- **Raising:** $⚠️ TODO — matches the total on Slide 13
- **Instrument:** ⚠️ TODO — SAFE (post-money cap) / convertible note / priced round
- **Valuation cap:** $⚠️ TODO
- **Minimum check:** $⚠️ TODO
- **Committed to date:** $⚠️ TODO — including founder capital
- **Target close:** ⚠️ TODO date

### What your cheque buys

- **Ownership** — a $⚠️ TODO cheque at a $⚠️ TODO cap is roughly ⚠️ TODO% of the company
- **Pro-rata rights** — the right to maintain your percentage in the next round ⚠️ TODO: confirm, and whether it applies above a minimum cheque
- **Quarterly investor updates** — progress, metrics, and what's not working

> **Speaker notes:**
> **This slide is the biggest structural difference between an angel deck and a VC deck.** A VC deck says "raising a seed round" and negotiates terms over subsequent weeks. An angel is often deciding *in the room*, and can't decide without knowing the instrument, the cap, and the minimum check. Leaving terms off the slide forces every interested angel to ask — and some won't.
>
> Naming a minimum check also does quiet qualification work: it tells a $10K angel they're looking at a syndicate, not a solo allocation, without an awkward conversation.
>
> **What each term means — you will be asked, and hesitating here reads badly.**
>
> - **SAFE** — *Simple Agreement for Future Equity.* The investor pays now and receives shares later, when a priced round happens. Not a loan: no interest, no maturity date, nothing that can be called. It lets you take money without agreeing a valuation today. Y Combinator publishes the standard document free; using it unmodified keeps legal costs near zero and means no angel needs a lawyer to read novel language.
> - **Valuation cap** — the highest company valuation their money will convert at. They get the cap price or the actual round price, **whichever is better for them**. If you later raise at $12M and their cap was $4M, their money buys shares as though the company were worth $4M — roughly three times what a new investor gets for the same cheque. That advantage is their compensation for going first.
> - **Post-money** — means ownership is calculable immediately: cheque ÷ cap. $50k at a $4M cap is 1.25%, full stop. Be clear-eyed that with post-money SAFEs each *additional* SAFE dilutes **you**, not the earlier holders.
> - **Minimum cheque** — the smallest allocation you will accept. It also does quiet qualification work: it tells a $10k angel they are looking at a syndicate rather than a direct allocation, without an awkward conversation.
> - **Committed to date** — money already in or verbally committed, founder capital included. Angels move in herds; a round that is partly filled is materially easier to fill.
> - **Pro-rata** — the *right, not the obligation,* to invest again in the next round to keep their percentage. Angels value this highly, because their returns depend on concentrating into the few winners. It costs you nothing today but consumes allocation later, which is why the usual compromise is to grant it only above a minimum cheque size.
>
> **Do the ownership arithmetic for them, on the slide.** A sophisticated angel will work out that a $50k cheque at a $4M cap is 1.25%; many will not bother, and some will get it wrong. Stating it signals you have thought about their side of the table.
>
> **Keep term-sheet detail off the slide.** Discount rates, MFN clauses and conversion mechanics belong in the SAFE document. Putting them here makes the round look like a negotiation rather than an invitation.
>
> ⚠️ TODO: Charles — a standard post-money SAFE is the lowest-friction instrument for a round of this shape, but the cap is a real decision. Worth a conversation before the first meeting, since it is hard to revise downward once quoted.
>
> ⚠️ TODO: decide whether pro-rata is offered, and above what cheque size. Under the post-money SAFE it is **not** automatic — it requires a separate side letter, so offering it is a deliberate act.

---

## Slide 15 — How This Returns Capital

**Headline:** ⚠️ TODO — the realistic exit paths.

**Likely acquirer categories:**

- **Frontier model providers** — Anthropic, OpenAI, Google DeepMind. Each already has an education initiative and each hits the same wall: a fluent tutor with no curriculum. **They also own the input cost — what we pay $5 for, they produce for a fraction of it.** The unit economics that make this viable for us are extraordinary for them
- **Publishers** — Pearson, McGraw Hill, Cengage: they own content and are structurally threatened by generated content
- **Learning platforms** — Coursera, Udemy, Chegg, Duolingo
- **LMS incumbents** — Instructure/Canvas, Anthology/Blackboard
- **Enterprise learning** — LinkedIn Learning, Docebo, Cornerstone
- **Big tech platform arms** — Microsoft, Google (Classroom / Workspace for Education)
- ⚠️ TODO: comparable transactions and multiples in this space

> **Speaker notes:**
> **This slide does not exist in a typical VC deck, and it must exist here.** A VC's returns come from portfolio construction and they'll model exits themselves. An angel is writing a personal check with no fund structure behind it and is asking, consciously or not, *"how does this become money again?"* Answering it unprompted is a mark of respect for their position.
>
> Don't overreach on numbers — naming plausible acquirer *categories* and why each is structurally motivated is more credible than a fabricated multiple.
>
> Note the publishers are simultaneously the competition named on the Market slide and the most motivated acquirers. That's a strength; say so.
>
> **Closing beat, after the last slide.** End on the demo rather than on the ask — hand them the link to the course they watched being built, and make the offer: *"Name any subject and I'll send you that course tomorrow."* It leaves them with something of their own rather than a request, and it gives you a reason to be back in their inbox within 24 hours without chasing.
>
> **The frontier-lab argument, made properly.** Three reinforcing reasons, in order of strength:
> 1. **Cost asymmetry.** Our ~$5 per course is what a lab *charges* for inference. Their internal cost to run the identical pipeline is a fraction of that. Every unit-economic constraint we operate under disappears for them — the same asset throws off far better margins in their hands than in ours. That is the textbook definition of an acquirer who can pay more for a business than it is worth standalone.
> 2. **Vertical integration.** Today we are their customer. Acquiring converts a customer's margin into their own product line.
> 3. **They already have the gap.** Every frontier lab is pushing into education and every one of them ships a fluent tutor with no curriculum, no mastery model, and no prerequisite structure — precisely the deficiency on the Problem slide. We are the missing layer, already built.
>
> **⚠️ Raising this invites the hardest question in the deck — have the answer ready before you say it.** *"If it's such a natural extension, why won't Anthropic just build it themselves?"* Answer in three parts, briefly:
> - **The patent.** Filed non-provisional, two independent claim sets covering generation and delivery separately. This is exactly the scenario the filing exists for, and it converts "build it" into "license or acquire it."
> - **Labs build horizontally.** They ship platforms and general capability; verticals are where they acquire rather than build. A curriculum graph with domain-specific verification is not on a frontier lab's roadmap.
> - **The hard part isn't generation.** It's the verified-figure pipeline, the separate-QA architecture, and the accumulated cross-linked graph — years of specific engineering that doesn't fall out of a better base model.
>
> Do **not** raise the frontier-lab category unless you can deliver that rebuttal cleanly. Unanswered, "why won't the labs just do this?" is the objection most likely to kill an angel's interest — it makes the whole company sound like a feature. Answered well, it does the opposite: it says the most sophisticated buyers in technology are structurally motivated to want you.
>
> **This makes the Defensibility slide load-bearing.** If the exit story leans on frontier labs, the patent stops being a nice-to-have and becomes the thing standing between you and being built around. Expect follow-up questions on claim scope.

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
- ⚠️ TODO: remaining 12–18 month milestones, tied to the Use of Funds milestone

### A4 — Patent detail

Non-provisional App. No. 19/756,145, filed 2026-07-28. Claim Set 1 covers AI-driven knowledge base generation; Claim Set 2 covers transitive-prerequisite adaptive delivery. The two claim sets are independently enforceable and licensable.

### A5 — The 1985 thesis: architectural correspondence

Source material for the Founder slide. Charles Irvine, *The Conceptual Knowledge System (CKS)*, master's thesis, University of Kansas, 1985. ⚠️ TODO: confirm exact month; scan in full.

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

**The two that carry the Founder slide:**

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

**Cross-sector comparison and capital gap (the Market slide):**

- WHO, *Global spending on health* (2024 report, data through 2022; $9.8T, 9.9% of global GDP) — https://www.who.int/teams/health-financing-and-economics/global-spending-on-health-report
- Gartner, *Worldwide IT Spending Forecast* ($5.43T, 2025) — https://www.gartner.com/en/newsroom/press-releases/2025-07-15-gartner-forecasts-worldwide-it-spending-to-grow-7-point-9-percent-in-2025
- SIPRI, *Trends in World Military Expenditure, 2024* ($2.718T) — https://www.sipri.org/publications/2025/sipri-fact-sheets/trends-world-military-expenditure-2024
- HolonIQ, *EdTech VC reached ~$2.4B for 2024, the lowest level of investment in a decade* — https://www.holoniq.com/notes/edtech-vc-reached-2-4b-for-2024-representing-the-lowest-level-of-investment-in-a-decade
- HolonIQ, *EdTech funding drops again in early 2025* — https://www.holoniq.com/notes/edtech-funding-drops-again-in-early-2025-fewer-deals-but-bigger-bets
- EdWeek Market Brief, *2024 Was the Worst Year for Ed-Tech VC Funding in a Decade* — https://marketbrief.edweek.org/financing-investment/2024-was-the-worst-year-for-ed-tech-vc-funding-in-a-decade-this-year-looks-even-worse/2025/05

**Caveat for diligence:** segment figures come from commercial market-research firms whose estimates vary widely by methodology (private tutoring alone is reported anywhere from ~$67B to ~$134B for 2025). The HolonIQ top-line and the U.S. government figures are the two most defensible numbers on the Market slide; lead with those and treat the rest as directional.

### A8 — The same market, viewed from the United States

Moved off the Market slide to keep it presentable. Use if an American angel asks for domestic figures.

| Segment | Annual spend |
|---|---|
| U.S. K–12 public schools | **~$1.0T** (FY2024, first year over $1T; ~$17.6K per pupil) |
| U.S. higher education institutions | **~$712B** total institutional expenditure |
| U.S. corporate & workplace training | ~$100B |
| U.S. private tutoring | ~$30B and growing double digits |

### A9 — Full candidate segment inventory

Working material behind the Business Model slide. **Direct-pay parents and learners — no procurement cycle:**

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

### A10 — Where the ~$5 per-course figure comes from

**Status: bottom-up estimate, not yet a measurement.** Cost instrumentation (`cost.py`, wired into both pipeline phases) now records real token usage and dollar cost on every generation, including runs that fail partway. Replace this section with measured figures after the next domain is created.

**Measured inputs — actual production graph, 64 domains:**

| | Total | Per course |
|---|---|---|
| Concepts | 2,202 | ~34 |
| Assessment questions | 6,844 | ~107 |
| Typed relationship edges | 14,580 | ~228 |
| Prerequisite edges | 9,420 | ~147 |
| Stored instruction | 16.4M chars (~4.1M tokens) | ~256K chars (~64K tokens) |

**Estimated model spend per course**, priced at Anthropic's **post-promotional** rates (Sonnet 5 at $3/$15 per MTok, Haiku 4.5 at $1/$5; cache reads 0.1×, cache writes 1.25×):

| Component | Estimate |
|---|---|
| Primary model output — instruction, figure construction code, edges, prerequisites, thinking | ~175K tokens → ~$2.60 |
| Primary model input — uncached | ~400K tokens → ~$1.20 |
| Primary model input — cache reads and writes | → ~$0.50 |
| QA model (assessments, figure assertions) | → ~$0.30 |
| **Total** | **~$4.60** |

Rounded to **~$5** for the slide. Roughly **$0.15 per concept**.

**Caveats to state if challenged:**

- Generated output exceeds stored output by roughly 2.7× — figure-repair loops, discarded candidates, and adaptive-thinking tokens are all billed but not all stored. The estimate accounts for this; a naïve estimate from stored content alone would be far too low.
- Voyage AI embeddings and reranking are **excluded** (they bypass LangChain's callback instrumentation). They are small relative to generation but non-zero.
- Infrastructure, Neo4j hosting, and human review time are excluded.
- Cost varies with domain size. A 45-concept course costs meaningfully more than a 20-concept one; quote the range ($3–8) rather than the point estimate if pressed on variance.
- **Sonnet 5's introductory rate ($2/$10) expires 2026-08-31.** This estimate deliberately uses the higher standard rate so it does not expire with the promo.

### A11 — Pre-revenue plan: conversion, then channels

**The finding that orders everything.** Google Analytics shows **86 active users** and 257 engaged sessions between 1 May and 22 August 2026. The production graph holds **15 accounts** and 25 enrolments. Roughly 84% of engaged sessions come from two locations — the founder, and the single power user.

The product works on the people who reach it. Almost nobody reaches it, and of those who do, most never create an account. **That is a conversion problem, not an awareness problem** — and publicity spent against a leaking funnel buys a bigger leak. Sequence the spend accordingly: conversion first, channels second.

**The conversion asset: a free prerequisite diagnostic.** A homeschool parent's recurring anxiety is *"does my child have gaps, and are they actually ready for algebra II?"* The transitive prerequisite graph answers exactly that, and nothing else on the market does. As a free, no-signup tool it demonstrates the differentiator instead of describing it, produces a result parents screenshot and share, captures email at peak intent, and ranks for the searches they really type. Generic free trials get ignored in this market; a diagnostic that tells a worried parent something true about their own child does not.

**Channels, in priority order.**

1. **Homeschool creators** — curriculum-review YouTube channels, Instagram practitioners, podcasters. Not celebrity influencers: trusted practitioners with niche, self-selected audiences. The offer is a *collaboration*, not a sponsorship — they publish a course under their own name, on their own school page, as an asset for their audience. Paid on revenue share, so the channel costs nothing until it converts and the creator only earns if their audience genuinely uses it. Budget a small guaranteed fee for the first two or three anchor partners, who take real reputational risk with no proof yet.
2. **Curriculum review gatekeepers** — Cathy Duffy Reviews is the market's canonical authority; Homeschool Buyers Club provides group-buying distribution. Slow to earn, disproportionate payoff.
3. **Co-ops and umbrella schools** — one director teaching eight children is a multi-seat sale *and* an endorsement to eight families.
4. **State associations and HSLDA** — vendor listings, newsletters, member channels.
5. **ESA and school-choice marketplaces** — several states now route public education funds to homeschool families through approved-vendor lists. Institutional process, not marketing spend, and it reaches *funded* demand. ⚠️ TODO: check the current state-by-state position; it is moving fast.
6. **Conventions** — vendor halls are where curriculum is actually chosen. A recorded generation demo runs well in that setting.
7. **Long-tail SEO** — the generated content is itself the asset. Publish complete sample units.

**What does not work here.** Paid ads as a primary channel — this audience is ad-skeptical and word-of-mouth driven. And treating homeschoolers as one market: classical, Charlotte Mason, unschooling, secular and religious segments differ in values and objections. Upper-level maths and science plays best with the **secular and rigour-focused eclectic** segments, which have the sharpest pain and the least AI scepticism.

**Creator relationships are a one-shot resource.** In a small community, a creator who sends their audience to something that disappoints will not promote again — and the other creators talk. This is the practical reason conversion work precedes outreach.

**Metrics to report, and to avoid.** Raw visits will be discounted, and rightly. Report diagnostic completions, accounts created, courses started and finished, returning users, and co-op conversations in progress. Ten families who finished a unit beats ten thousand visitors, and an angel will say so.
