# Pitch Deck — Open Items

Working list for `qlaudia_pitch_deck.md`. Every item here also appears inline in the deck as a `⚠️ TODO` marker, so the two stay findable together.

After editing the markdown, regenerate the PowerPoint:

```bash
cd pitch_deck && .venv/bin/python md2pptx.py
```

## Slide index

Numbers match PowerPoint exactly. Markdown headings carry them too (`## Slide 12 — Use of Funds`),
and the converter checks each against the position it actually renders at — a stale number is
reported at build time rather than shipped. They will still shift if the deck's structure changes
(item 16 would renumber everything after slide 2), and appendix numbers move whenever a section
grows onto another continuation slide. Names are given alongside for that reason.

| # | Slide | | # | Slide |
|---|---|---|---|---|
| 1 | *(title)* | | 15 | Appendix divider |
| 2 | Education Is the Largest Untransformed Market | | 16 | A1 — Competition |
| 3 | Educational Spend and the Emerging Alternative | | 17 | A2 — Technical architecture |
| 4 | The Problem | | 18 | A3 — Roadmap |
| 5 | The Solution | | 19 | A4 — Patent detail |
| 6 | Founder: I Designed This System in 1985 | | 20 | A5 — Thesis correspondence |
| 7 | Watch It Build a Course *(demo)* | | 21–23 | A6 — Thesis quotations |
| 8 | Why Now | | 24–25 | A7 — Market sources |
| 9 | Defensibility | | 26 | A8 — U.S. market detail |
| 10 | Business Model & First Customers | | 27–28 | A9 — Segment inventory |
| 11 | Traction | | 29–30 | A10 — Cost derivation |
| 12 | Use of Funds | | 31–33 | A11 — Pre-revenue plan |
| 13 | The Ask | | | |
| 14 | How This Returns Capital | | | |

**13 pitch slides**, plus title, appendix divider and appendix.

---

## Blocking — the deck cannot go in front of an angel without these

**Do these in order.** Slide 12's numbers determine slide 13's ask; settling the ask first means redoing it.

- [ ] **1. Slide 12 · Use of Funds — mostly done; the runway number is open.**
      Buckets and total are set: schools and sponsors $15k, purchasing $5k, hardening $10k, legal and formation $3k, operating runway $5k — **$38,000 total**. The milestone is set too: three sponsored schools live, audiences arriving, paying customers through checkout.
      **Still open: months of runway.** Think hard about this one. Recruiting SMEs, generating and reviewing their courses, launching, waiting for an audience, building purchasing and converting is realistically four to six months of work. Three months would mean missing the milestone in front of the people who funded it, which is worse than asking for a longer runway now.
      Founder takes no compensation — retired with independent income. ⚠️ Add that line to the slide so the blank reads as a decision rather than an oversight.

- [ ] **2. Slide 13 · The Ask — the terms.** Two blocks to fill.

      **The terms:** raise amount *(must equal the total on slide 12)*, instrument (a post-money SAFE is lowest-friction for a round this shape), valuation cap, minimum cheque, committed-to-date including founder capital, target close.

      **What your cheque buys:** the ownership arithmetic spelled out (cheque ÷ cap — e.g. $50k at a $4M cap is 1.25%), whether pro-rata is offered and above what cheque size, and the investor-update cadence.

      Angels frequently decide in the room and cannot without these. Two decisions inside this item deserve real thought:
      - **The cap** is hard to revise downward once quoted, and it only bites in the case where you succeed — the gap between a $3M and a $6M cap is millions of dollars of your ownership at a good exit.
      - **Pro-rata is not automatic** under the post-money SAFE; it needs a separate side letter. Granting it costs nothing today but consumes allocation in your next round, which is why the usual compromise is to offer it only above a minimum cheque size.

      Definitions of every term are in slide 13's speaker notes, written for reading aloud under questioning.
      **Gated by item 19** — a SAFE cannot be issued by an LLC, so the entity has to exist first. Raise amount is now known: **$38,000** (slide 12 total).

- [ ] **3. Slide 10 · Business Model — the numbers behind the model.**
      The model and the split are settled (item 17): founding sponsors keep **80% for life**, later cohorts at a standard rate. What is still open: **which schools go first and which SMEs to approach**, by name; the bottom-up number — schools × audience × conversion × price; and whether 80% is of **gross or net** after payment processing.
      Also owed: a **review workflow that makes "blessing" meaningful**. An SME who skims and signs is exposed if the course is wrong, and their credibility burns before yours. Being able to describe the workflow is itself a recruiting asset.

- [ ] **4. Slide 7 · Demo — record it.**
      Full run: typing the course description → advisor exchange → syllabus review → pipeline → finished course. Time-lapse the long stretches; keep the input and review at real speed. Keep the raw capture for diligence.
      - [ ] **Read the course before recording.** The 5–8 concepts that appear on camera, plus anything touching deal terms, dilution, or valuation caps. ~20 minutes. Pre-generating exists so you can inspect before they do.
      - [ ] Still screenshots as a fallback for rooms without video, and for the send-after deck.

- [ ] **5. Slide 6 · Founder — name an advisor, and answer key-person risk.**
      The natural candidate is a **first school sponsor** who works out — an SME with an audience, on a small vesting equity grant. That closes the credibility gap and deepens a distribution partner in one conversation.
      **Recruit for the solo-founder risk, not for age optics.** Of the three things an angel actually worries about — time horizon, key-person risk, succession — two are solo-founder problems that age merely makes louder. Someone brought in to fix appearances will read as exactly that, and the equity is permanent.
      **Have the "what if you stop" answer ready:** the patent and the generated corpus are transferable assets with value independent of the founder. That defuses most of the concern in one sentence. Don't raise age unprompted; visible ease with it is a stronger signal than any argument.
      ⚠️ TODO: decide advisor vs. named first hire vs. co-founder. An advisor plus a documented succession answer covers this round; a co-founder is worth the equity only if the goal is a genuine partner.

---

## Content gaps

- [ ] **6. Slide 11 · Traction** — institutional conversations, pilots, or LOIs, if any exist.
- [x] **6a. Slide 11 · Traction — add the forum experiment.** *(done)* Independent of item 17: it is the only distribution evidence that exists, and it belongs in the deck whichever beachhead wins.
      One post to an arrhythmia forum about Charles's own case produced the site's best traffic and its only power user. Every other forum post was removed by moderators as advertisement. The lesson is that moderators judge *standing*, not content — which is why the model is "members publish their own school," not "we post in forums." An angel who knows online communities will ask about moderation the moment forums are mentioned; having already run the experiment is a far stronger answer than a plan that has never met a moderator.
- [ ] **7. Slide 14 · How This Returns Capital** — comparable transactions and multiples for the acquirer categories.
- [ ] **8. Slide 7 · Watch It Build a Course** — pull one genuinely impressive generated figure into the demo capture. *(The standalone Pipeline slide was cut; its figure-verification argument now lives on Defensibility and in the demo.)*
- [ ] **9. Slide 18 · Appendix A3 (Roadmap)** — remaining 12–18 month roadmap milestones, tied to the Use of Funds milestone.
- [ ] **10. Slides 31–33 · Appendix A11 (Pre-revenue plan)** — current state-by-state position on ESA / school-choice vendor marketplaces. Moving fast; worth checking close to the pitch.

---

## Verification — things that are true but unconfirmed, or will drift

- [ ] **11. Slide 8 · Why Now — replace the estimated cost with a measured one.**
      Blocked on a code fix: steps 3 and 5 invoke with `config={"callbacks": [logger]}`, which *replaces* the inherited callback list instead of appending, so their usage never reaches the cost handler. Reported totals currently understate spend by roughly 40%.
      "We measured it" is materially stronger than "we estimated it," and you are one pipeline run away from being able to say it.

- [ ] **12. Slide 11 · Traction — refresh production figures the week of the pitch.** They move.
      ```bash
      cd qlaudia_server && .venv/bin/python scripts/list_user_enrollments.py --prod
      ```
      Build-side counts come from a direct query against the production graph.

- [ ] **13. Slides 6 and 20 · Founder / Appendix A5** — flat scans of the 1985 thesis abstract and the §1.3 "Approach and Scope" page. Phone photos will not hold up projected. Confirm the exact month of the thesis.

- [ ] **14. Slide 9 · Defensibility** — settle the exact wording if asked about the outstanding IDS and inventor declaration.

- [ ] **15. Slide 16 · Appendix A1 (Competition)** — confirm which competitors actually come up in real conversations. The grid is currently generic.

---

---

## Open decisions

- [ ] **16. Slides 2–3 · Market slide length.** The adjacent-spend bullets pushed slide 2 into needing a companion, slide 3. Moving them to the appendix would fold the two back together. Cheap to do now — the converter numbers slides by position, so nothing downstream needs renumbering.

- [x] **17. Beachhead — RESOLVED: sponsored schools.**

      Not a vertical, a *mechanism*. Qlaudia generates a course; a subject-matter expert reviews it, publishes it under their own name as a school, and promotes it to their own audience for a share of sales. Verticals compete on evidence rather than being chosen up front — arrhythmia is a school, 7–12 maths is a school.

      Why it beat both earlier candidates: it makes the supply side nearly free (review is hours, writing is months), it solves the standing problem structurally (an SME is a member, Qlaudia is a vendor), and it is a portfolio bet rather than a single wager.

      Consequences already applied: the Business Model slide rewritten, the Traction slide leads with 7 live schools and the forum experiment, Use of Funds gains course purchasing as its own bucket, and Appendix A11 rebuilt around SME recruitment.

- [ ] **18. Who to approach first — start with people who already know you.**
      Thirty years of Kansas City technology colleagues (Sprint, DST, Cadence, TreviPay), many now senior, some with liquidity. Nobody who has watched your work for decades will discount you on age, and at $38,000 this round is one or two people rather than a syndicate. That makes *who* far more important than *how many*, and it routes around the age question entirely rather than arguing with it.
      ⚠️ TODO: name the first five to call.

---

## Legal, formation and accounting

- [ ] **19. Form the entity — do this before taking a dollar.** ← *gates item 2*
      **A SAFE cannot be issued by an LLC.** The documents convert into stock, LLC investors receive K-1s and can owe tax on income they never received, and QSBS — often an angel's single biggest tax incentive — requires C-corp stock. Any later VC round requires a Delaware C-corp regardless.
      Charles Irvine Enterprises LLC is now effectively clean: Top Gun Pool League, Mozart, Opera and Academy-courses.com are all obsolete and retirable. Converting would preserve the 2017 formation date that supports the pre-ChatGPT provenance on slide 6, but bespoke conversion costs several times a fresh formation. **On a $38k round, form fresh** — the 2017 date is provable from LLC records, domain registrations and public GitHub history.
      - [ ] Delaware C-corp via Stripe Atlas or Clerky (a few hundred dollars)
      - [ ] **Assign the IP to it** — patent App. No. 19/756,145 explicitly, plus code, content, trademarks, domains. This gets diligenced; a patent left in a personal or LLC name is a finding
      - [ ] Founder stock issued, then the **83(b) election — 30-day hard deadline from issuance, no relief if missed.** The most common expensive founder mistake there is
      - [ ] Decide the securities path: Reg D **506(b)** (no general solicitation — you may not publicly advertise that you are raising) or **506(c)** (may advertise, but must *verify* accreditation)
      - [ ] Business bank account in the new entity's name
      - [ ] Confirm the retired projects left no users, payments or open obligations behind — "no liabilities, and here's why" is worth being able to say flatly
      - [ ] Keep **academy-courses.com** registered and pointed at Qlaudia; it is cheap evidence for the 2017 provenance

- [ ] **20. After the raise opens.**
      Form D with the SEC within 15 days of first sale; state blue-sky notices where investors reside; a cap table that is actually maintained; bookkeeping from day one (the cost instrumentation is genuinely useful here as COGS data). Ask an accountant about the **R&D tax credit** — startups can offset payroll taxes with it, and there are years of build behind you.

- [ ] **21. Product-side legal, before purchasing ships.**
      - **Payments make you a marketplace.** Paying sponsors a share means handling third-party funds — likely Stripe Connect rather than plain Stripe, and 1099s for any sponsor paid over $600 in a year. This shapes the integration, so settle it before building
      - **Medical content liability.** The arrhythmia school is patient-facing health information and needs disclaimers written by someone who does this professionally
      - **Minors.** A 7–12 maths school means under-13 users are plausible — that is COPPA, with real requirements on parental consent and data collection. FERPA applies if you ever sell into schools
      - Terms of service and a privacy policy, given auth, user data and imminent payments

## Known weak points to have answers for

Not edits — things an angel may probe, where the honest answer is already in the speaker notes.

- **Zero quiz questions answered in production.** *(slides 9 and 11)* Competency is 0% for every user; progress is self-marked "got it." This is a signal about *who is using it*, not a defect — interest-driven readers do not self-assess, and forcing them to would likely reduce engagement. Have the answer ready if asked; no need to volunteer it.
  Two corollaries. **It bears on item 17:** assessment matters most for homeschool families in compliance states, who need documented evidence for portfolio review, and least for patients — so distribution evidence points at patients while product depth points at homeschool. And **intent versus discoverability produce identical data**: the quiz is a small `?` icon in the concept header. If users open quizzes and abandon them, that is intent; if nobody opens one at all, discoverability is a factor.
- **The funnel, not awareness, is the problem.** *(slide 11)* 86 visitors over four months produced 15 accounts, and most engaged sessions come from two locations. The product works on people who reach it; almost nobody reaches it.
- **No prior venture-backed company.** *(slide 6)* The true answer that lands: a working end-to-end pipeline and a filed non-provisional patent, built solo.
- **"Why won't the frontier labs just build it?"** *(slide 14)* Raised by slide 14's lead acquirer category. Three-part rebuttal is in that slide's notes — do not raise the category unless you can deliver it cleanly.
- **Founder age.** *(slide 6)* Slide 6 makes a 1985 start date unavoidable. The counter is the slide's own argument: two AI paradigms of direct experience, not a guess about which one is different.
