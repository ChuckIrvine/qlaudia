# Pitch Deck — Open Items

Working list for `qlaudia_pitch_deck.md`. Every item here also appears inline in the deck as a `⚠️ TODO` marker, so the two stay findable together.

After editing the markdown, regenerate the PowerPoint:

```bash
cd pitch_deck && .venv/bin/python md2pptx.py
```

## Slide index

Numbers match PowerPoint exactly. Markdown headings now carry them too (`## Slide 13 — Use of
Funds`), and the converter checks each against the position it actually renders at — a stale
number is reported at build time rather than shipped. They
stay correct as slides are added or split. They will shift if the deck's structure
changes (item 16 would renumber everything after slide 2), and appendix numbers move
whenever an appendix section grows onto another continuation slide. Names are given
alongside for that reason.

| # | Slide | | # | Slide |
|---|---|---|---|---|
| 1 | *(title)* | | 16 | Appendix divider |
| 2 | Education Is the Largest Untransformed Market | | 17 | A1 — Competition |
| 3 | The Three Numbers That Matter | | 18 | A2 — Technical architecture |
| 4 | The Problem | | 19 | A3 — Roadmap |
| 5 | The Solution | | 20 | A4 — Patent detail |
| 6 | Founder: I Designed This System in 1985 | | 21 | A5 — Thesis correspondence |
| 7 | Watch It Build a Course *(demo)* | | 22–24 | A6 — Thesis quotations |
| 8 | This Is a Pipeline, Not a Prompt | | 25–26 | A7 — Market sources |
| 9 | Why Now | | 27 | A8 — U.S. market detail |
| 10 | Defensibility | | 28–29 | A9 — Segment inventory |
| 11 | Business Model & First Customers | | 30–31 | A10 — Cost derivation |
| 12 | Traction | | 32–34 | A11 — Pre-revenue plan |
| 13 | Use of Funds | | | |
| 14 | The Ask | | | |
| 15 | How This Returns Capital | | | |

---

## Blocking — the deck cannot go in front of an angel without these

**Do these in order.** Slide 13's numbers determine slide 14's ask; settling the ask first means redoing it.

- [ ] **1. Slide 13 · Use of Funds — the numbers.**
      Amounts for the three buckets (distribution / hardening / runway), months of runway, and the milestone the round reaches. The milestone is the important one: *what is measurably true after this money that isn't true today?*

- [ ] **2. Slide 14 · The Ask — the terms.** Two blocks to fill.

      **The terms:** raise amount *(must equal the total on slide 13)*, instrument (a post-money SAFE is lowest-friction for a round this shape), valuation cap, minimum cheque, committed-to-date including founder capital, target close.

      **What your cheque buys:** the ownership arithmetic spelled out (cheque ÷ cap — e.g. $50k at a $4M cap is 1.25%), whether pro-rata is offered and above what cheque size, and the investor-update cadence.

      Angels frequently decide in the room and cannot without these. Two decisions inside this item deserve real thought:
      - **The cap** is hard to revise downward once quoted, and it only bites in the case where you succeed — the gap between a $3M and a $6M cap is millions of dollars of your ownership at a good exit.
      - **Pro-rata is not automatic** under the post-money SAFE; it needs a separate side letter. Granting it costs nothing today but consumes allocation in your next round, which is why the usual compromise is to offer it only above a minimum cheque size.

      Definitions of every term are in slide 14's speaker notes, written for reading aloud under questioning.

- [ ] **3. Slide 11 · Business Model — pick one motion.**
      One primary revenue motion, a price point, the realistic first ten customers, and the bottom-up number (beachhead × price × penetration). Five listed motions reads as none.
      Price anchor *(if the beachhead stays homeschool)*: this buyer already pays for outsourced online courses and $40–60/hr tutors — not free Khan Academy.
      **Gated by item 17** — settle the beachhead first, or this gets answered twice.

- [ ] **4. Slide 7 · Demo — record it.**
      Full run: typing the course description → advisor exchange → syllabus review → pipeline → finished course. Time-lapse the long stretches; keep the input and review at real speed. Keep the raw capture for diligence.
      - [ ] **Read the course before recording.** The 5–8 concepts that appear on camera, plus anything touching deal terms, dilution, or valuation caps. ~20 minutes. Pre-generating exists so you can inspect before they do.
      - [ ] Still screenshots as a fallback for rooms without video, and for the send-after deck.

- [ ] **5. Slide 6 · Founder — name an advisor.**
      The one real gap on slide 6. A recognised figure from the chosen beachhead community — homeschool or patient advocacy — on a small vesting equity grant closes the credibility gap *and* creates a distribution partner (A11) in one conversation.
      **Profile depends on item 17.** A patient-education advisor looks nothing like a homeschool one.

---

## Content gaps

- [ ] **6. Slide 12 · Traction** — institutional conversations, pilots, or LOIs, if any exist.
- [ ] **6a. Slide 12 · Traction — add the forum experiment.** Independent of item 17: it is the only distribution evidence that exists, and it belongs in the deck whichever beachhead wins.
      One post to an arrhythmia forum about Charles's own case produced the site's best traffic and its only power user. Every other forum post was removed by moderators as advertisement. The lesson is that moderators judge *standing*, not content — which is why the model is "members publish their own school," not "we post in forums." An angel who knows online communities will ask about moderation the moment forums are mentioned; having already run the experiment is a far stronger answer than a plan that has never met a moderator.
- [ ] **7. Slide 15 · How This Returns Capital** — comparable transactions and multiples for the acquirer categories.
- [ ] **8. Slide 8 · This Is a Pipeline, Not a Prompt** — pull one genuinely impressive generated figure as the slide visual. One good figure does the whole slide's job.
- [ ] **9. Slide 19 · Appendix A3 (Roadmap)** — remaining 12–18 month roadmap milestones, tied to the Use of Funds milestone.
- [ ] **10. Slides 32–34 · Appendix A11 (Pre-revenue plan)** — current state-by-state position on ESA / school-choice vendor marketplaces. Moving fast; worth checking close to the pitch.

---

## Verification — things that are true but unconfirmed, or will drift

- [ ] **11. Slide 9 · Why Now — replace the estimated cost with a measured one.**
      Blocked on a code fix: steps 3 and 5 invoke with `config={"callbacks": [logger]}`, which *replaces* the inherited callback list instead of appending, so their usage never reaches the cost handler. Reported totals currently understate spend by roughly 40%.
      "We measured it" is materially stronger than "we estimated it," and you are one pipeline run away from being able to say it.

- [ ] **12. Slide 12 · Traction — refresh production figures the week of the pitch.** They move.
      ```bash
      cd qlaudia_server && .venv/bin/python scripts/list_user_enrollments.py --prod
      ```
      Build-side counts come from a direct query against the production graph.

- [ ] **13. Slides 6 and 21 · Founder / Appendix A5** — flat scans of the 1985 thesis abstract and the §1.3 "Approach and Scope" page. Phone photos will not hold up projected. Confirm the exact month of the thesis.

- [ ] **14. Slide 10 · Defensibility** — settle the exact wording if asked about the outstanding IDS and inventor declaration.

- [ ] **15. Slide 17 · Appendix A1 (Competition)** — confirm which competitors actually come up in real conversations. The grid is currently generic.

---

## Open decisions

- [ ] **16. Slides 2–3 · Market slide length.** The adjacent-spend bullets pushed slide 2 into needing a companion, slide 3. Moving them to the appendix would fold the two back together. Cheap to do now — the converter numbers slides by position, so nothing downstream needs renumbering.

- [ ] **17. Beachhead: patient education vs. homeschool.** *(rewrites slides 11, 12 and 32–34)* ← *decide before item 3*

      The deck currently names upper-level homeschool maths and science, reasoned from first principles with **no evidence behind it**. Patient education is the only thing that has actually worked, and it is not in the deck at all.

      **Evidence for patient education**
      - The one validated distribution event: a post to an arrhythmia forum about Charles's own case, linking the school. Produced the site's best traffic and its only power user — five courses, 224 concepts, all completed, ~23h engagement.
      - The courses already exist ("Heart Arrhythmias for Patients and Family", 8 courses, plus *Understanding Your Pacemaker Report*).
      - Prerequisite depth is real and *felt* — you cannot understand AFib without conduction, or conduction without heart structure. That is the differentiator, experienced directly by the learner.
      - Genuinely underserved. Homeschool maths has Khan Academy, Saxon, IXL, Thinkwell; "understand your arrhythmia" has essentially nothing structured between a pamphlet and a journal article.
      - Motivation is extreme — their health depends on it.
      - The `School` structure already fits: one school per condition.

      **The moderation finding, which shapes the whole model**
      Every forum post other than the arrhythmia one was removed by moderators as advertisement. Moderators were not judging the content — they were judging *standing*. Same offer, member vs. stranger, opposite outcome. Two consequences: never post as Qlaudia anywhere; and the model is not "we post in forums" but "patients publish their own school and share it themselves." The rejections are also a positive signal — a well-policed community is exactly why the one successful post converted so well.

      **Arguments against / unresolved**
      - Willingness to pay is unproven; patients often expect education free from their care team.
      - Accuracy and liability stakes are materially higher than homeschool maths.
      - The authenticity does not scale from Charles — he has one condition, so every other community needs its own advocate.

      **Possible resolution worth costing:** free to patients, monetised institutionally — hospitals, device manufacturers, patient advocacy organisations. Keeps the advocate's motives clean, which is what makes the channel work at all. Also avoids the real risk that a revenue share reads as monetising a support group.

      **If this changes:** Slide 11 is rewritten around patient education with homeschool demoted to expansion; slide 12 gains the forum experiment as distribution evidence; Appendix A11 (slides 32–34) is rebuilt around condition communities and advocacy organisations.

- [ ] **18. Co-founder, or advisor plus a GTM hire?** *(affects slides 6 and 13)* ← *also gated on item 17*

      The gap is not technical — the product is built. It is distribution, and specifically *standing*: the forum experiment showed Charles cannot be a legitimate member of every community he needs to reach. That is not solvable by working harder.

      **The spectrum**, cheapest first: advisor (0.25–1%, vesting) → fractional GTM → first hire funded by the round → co-founder (10–40% and a permanent decision partner).

      For the deck specifically, *advisor now + named GTM hire in the use-of-funds plan* delivers most of the investor benefit at a fraction of the cost, and does not require finding a peer under fundraising time pressure.

      **Do not recruit a co-founder to fix a slide.** Equity is permanent. A co-founder is right if the goal is a genuine partner to share decisions and load — a personal question as much as a strategic one. Also worth resisting "or two": one to three founders is a large dilution and materially harder coordination.

      Where to look: the 40-year operator network, or — more structurally — someone with real standing inside the chosen beachhead community who is also operationally capable.

---

## Known weak points to have answers for

Not edits — things an angel may probe, where the honest answer is already in the speaker notes.

- **Zero quiz questions answered in production.** *(slides 8 and 12)* Competency is 0% for every user; progress is self-marked "got it." This is a signal about *who is using it*, not a defect — interest-driven readers do not self-assess, and forcing them to would likely reduce engagement. Have the answer ready if asked; no need to volunteer it.
  Two corollaries. **It bears on item 17:** assessment matters most for homeschool families in compliance states, who need documented evidence for portfolio review, and least for patients — so distribution evidence points at patients while product depth points at homeschool. And **intent versus discoverability produce identical data**: the quiz is a small `?` icon in the concept header. If users open quizzes and abandon them, that is intent; if nobody opens one at all, discoverability is a factor.
- **The funnel, not awareness, is the problem.** *(slide 12)* 86 visitors over four months produced 15 accounts, and most engaged sessions come from two locations. The product works on people who reach it; almost nobody reaches it.
- **No prior venture-backed company.** *(slide 6)* The true answer that lands: a working end-to-end pipeline and a filed non-provisional patent, built solo.
- **"Why won't the frontier labs just build it?"** *(slide 15)* Raised by slide 15's lead acquirer category. Three-part rebuttal is in that slide's notes — do not raise the category unless you can deliver it cleanly.
- **Founder age.** *(slide 6)* Slide 6 makes a 1985 start date unavoidable. The counter is the slide's own argument: two AI paradigms of direct experience, not a guess about which one is different.
