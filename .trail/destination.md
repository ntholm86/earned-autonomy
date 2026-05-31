# Destination — pea-website

*Written by agent after Vision run, 2026-05-26. Updated 2026-05-27 (iter-39 Vision run). Updated 2026-05-27 (iter-51 Vision run — skills-first shift). Operator commits when it reads right.*

---

## The destination

A single-page public website that is the credible intellectual face of the Principles of Earned Autonomy ecosystem — legible to someone arriving cold from GitHub or Zenodo, and equally useful as a link sent to someone with partial context.

It is not a product page. It is not a personal portfolio. It is an intellectual position made accessible.

**The demonstration lives in the trail, not on the page.** The build history, Vision dialogues, and Improve iterations are committed to `.trail/` and verifiable against the git log. That is Observable Autonomy working as designed. The page itself serves its audience — it does not explain its own construction.

---

## Reader

**Primary: the non-technical reader arriving cold** — someone thinking seriously about AI delegation who has no prior PEA context. This is the design constraint. If they don't get the point without reading every paragraph, the page has failed.

**Secondary: the informed reader** — someone sent here with context, or a technical evaluator arriving from GitHub/Zenodo. They get value from the depth of the content but do not constrain design decisions.

The shift from "both equally" (session-001 Vision) was confirmed in the 2026-05-26 Vision run.

---

## Structure

**[REVISED iter-51 — 2026-05-27: skills-first shift]**

**Prior structure (iter-39, now superseded):**
~~1. The Principles — as the intellectual core~~
~~2. The Skillset — as the concrete implementation~~
*The operator confirmed this inverts: skills are now the entry point; principles are the explanation behind them.*

**Current structure:**

1. **Hero** — unchanged. "You're delegating real work to AI. Stay accountable for the work." Problem-framing remains the entry point.

2. **The Skills** — primary content section. Moves above Principles. The reader should land on this before the framework.
   - **Trail first** — "what most realize they are missing right now." The recognition hook.
   - **Intent second** — devs feel this problem: the agent goes somewhere sideways because it interpreted the brief literally.
   - **Improve third, with 2× visual depth** — this is where work actually gets done. The section should show: the loop itself (read trail → examine → challenge → decide → one change → verify → reflect), the lineage (started as Kaizen from Toyota Kata; v2 split into Kaizen/Kaikaku/Hansei; v3 unified), and the evidence (200+ iterations on itself, two full self-rewrites). Improve is not a card — it is a subsection.
   - **Vision fourth** — the piece that sets the destination. The agent needs to know where it's going; Vision is how you tell it. Direction/goal/mission/destination are all the same thing here.
   - **Retrospect and Probe** — supporting roles, not removed. Keep as cards below Vision.

3. **The Principles** — moves below Skills. Reframed as "why the skills are built this way" — the intellectual grounding you reach *after* deciding the skills are worth trying. Commander's Intent, Observable Autonomy, Convergence Is Silence remain, but they now *explain the skills*, not precede them.

The page is no longer "framework with implementation." It is "tools that solve today's problems, with the framework that explains why they work."

**Phrase candidate (Vision run, 2026-05-27):** "Delegate to AI. Own the work." — operator to confirm or adjust. Six words, two imperatives, captures the tension the page is built around. Potential use: hero subtitle, section label, or meta description replacement.

The harness protocol remains out of scope.

## What success looks like

A developer arriving cold should:
- Recognize their own problem in the Trail or Intent card **within 3 seconds** — without reading
- Understand what Improve does and feel the shape of the loop within 30 seconds — by scanning, not reading
- Feel **recognition + intrigue**: "I've been trying to solve this, and this names it" — not impressed, not informed, *found*

**Emotional destination (confirmed 2026-05-27, reaffirmed iter-51):** the primary reader is a developer who has already felt the gap — the audit trail they don't have, the brief that went sideways, the run they can't verify. The page reaches them at the recognition point, not at the framework entry point.

"Serious and credible, not promotional" remains a valid constraint — but credibility is what makes recognition stick, not how recognition is achieved.

---

## Tone

Warmer and more accessible than POSITION.md — written for a non-technical reader who is thinking seriously about AI delegation, not an academic evaluating a framework.

**Stick with the PEA terms.** Commander's Intent, Observable Autonomy, Convergence Is Silence, delegability, Autonomous Reasoning Fidelity — these are used, but explained when introduced. The vocabulary is a thinking tool, not a credential barrier.

Epistemic register: honest and direct. Not promotional. Claims are grounded. The author is confident but not boastful. The work is real and the page reflects that.

---

## What is rejected

- Personal CV / professional portfolio framing
- Promotional or sales-page tone
- Connecting principles → skills → harness as a single technical stack narrative
- Any harness protocol content (deferred)
- Self-referential proof section in any form (removed iter-8; the demonstration lives in the trail)
- "Both audiences equally" as a design constraint (non-technical reader is now primary)
- **Principles-first page structure** (reversed iter-51 — skills are the entry point, principles explain why the skills are built the way they are)

---

## Colour system (revised — iter-36, confirmed 2026-05-27)

**Dark, not light.** The light palette (session-007/008 through iter-35) was reversed in iter-36 by operator request and confirmed as settled in the Vision run of 2026-05-27.

*Historical note: the prior ruling was "Light, not dark. The Monokai dark palette was explicitly rejected." That ruling was reversed by operator direction in iter-36. The [!REVERSAL] record is in the iter-36 trail entry.*

**Dark canvas palette (current):**
- `--bg: #1e2030` — deep navy-charcoal
- `--bg-elev: #252a3a` — elevated surface (cards)
- `--ink: #e4e7ec` — off-white body text (~12:1 contrast)
- `--muted: #a8b1c2` — warm grey (~7:1 contrast)
- `--rule: #2f3548` — subtle border

**Semantic colour roles (iter-38 — type determines colour, not section geography):**

| Role | Colour | Hex |
|---|---|---|
| `.label`, `.trail-marker` — structural announcements | coral | `#f48a8a` |
| `code`, `.mono`, filenames — technical identifiers | amber | `#e7c97a` |
| `a`, `.btn`, `.icon`, nav hover — action / navigation | teal | `#7fd1c5` |
| `em` inline emphasis — conceptual highlight | lavender | `#c4a7e7` |
| `.card-accent` border, `.numeral-circle` — evidence / verified | sage | `#a3d6a7` |

**The invariant:** element type determines colour globally. A link is teal everywhere. Section geography does not change colour semantics.

---

## What is still open

- **Recognition + intrigue — not yet achieved.** The page must deliver the instant feeling of "this is what I've been looking for — to safely delegate work to AI." Currently unsatisfying across all three dimensions: visual clarity, contextual clarity, copy. Operator verbatim (2026-05-27): *"it does not give this instant feeling of solving that hard problem."*
  - The structural fix: the hook must name the reader's problem *and* promise relief before any framework language appears. The hero currently leads with pain before relief.
  - The design still relies on text being read rather than structure being seen.
- **Visual verification not done.** No browser render check since the dark theme (iter-36). Contrast ratios for `--sage` and `--lavender` on `--bg` are estimated, not measured. Mobile viewport untested.
- **GitHub Pages push** — blocked by the clarity problem above.

---

## Vision update — iter-59 (2026-05-28)

**Skills section restructured. Two new direction claims confirmed by operator.**

### New framing: skills map directly to principles

The operator confirmed that the three immediate-use skills each enact one principle:

- **Intent → P1 Commander's Intent** — forces the agent to state its interpretation before acting
- **Trail → P2 Observable Autonomy** — enforces the audit trail
- **Improve → P3 Convergence Is Silence** — one change, one iteration, verified and logged

This connection was invisible on the page. It is now the label on each card.

### Two-tier skill structure

The six skills split into two tiers by when the user needs them:

- **Tier 1 (immediate):** Intent, Trail, Improve — these solve recognisable problems from day one
- **Tier 2 (deferred):** Vision, Retrospect, Probe — memory model, higher awareness, self-reflection, ARF. The need is there; it becomes visible once the first tier is running.

### Order: Intent → Trail → Improve (supersedes retro-003 rule 9)

Prior retrospect rule 9 specified Trail → Intent. The operator has confirmed: principle order (P1 → P2 → P3) is the correct ordering. Intent comes first because Commander's Intent is P1.

### Card interaction: title-as-link (not whole-card-as-link)

Clicking the skill title takes you to the skill on GitHub. The card itself is not a link. This resolves the Improve inconsistency (Improve was never an a.card) and matches the operator's stated preference.

### Label color: coral → lavender

Red labels communicate danger/error. Labels are now lavender (conceptual emphasis). Trail markers ([!DECISION], [!REALIZATION]) are now amber (technical identifiers). Coral is no longer the dominant UI color.

---

## Vision update — iter-84 — 2026-05-28

**Convergence criterion is undefined by the operator.**

The prior vision.md stated: "What success looks like: recognition + intrigue — 'I've been trying to solve this, and this names it.'" That framing was agent-generated in earlier Vision runs. The operator has never confirmed it as their own test.

When asked directly what done looks like during the iter-84 session, the operator said: "I am not sure what done actually looks like."

**[!REALIZATION]** The loop has been operating without an operator-confirmed convergence criterion. The emotional destination claim ("recognition + intrigue") is an agent inference, not an operator statement. It may be correct — but it has not been confirmed.

**Open question for the operator:** What would a reader have to say or do after visiting this page for you to feel the page has done its job? Is there a specific reaction, a specific type of person, a specific action (installing the skills, sharing the link, reaching out)?

Until the operator can answer this, convergence cannot be declared. This is not a failure — it means the page is still in the exploration phase, not the convergence phase.

---

## Destination update — iter-132 — 2026-05-28

**The `#trail` section is repurposed: from teaching trail-format to standing as evidence-of-origin.**

It previously showed three verbatim `audit-trail.md` entries as "what an entry looks like" — a format demonstration. The operator redirected it: the section's purpose is to be the *empirical credential of the skillset itself*. The skills are not top-down design; they are the convergent output of running the Improve loop on itself 200+ times, through its own evolution (Kaizen from Toyota Kata → split into Kaizen/Kaikaku/Hansei → unified Improve), stopped only when multiple independent AI model families each found nothing left to change while the principles held.

Operator framing (2026-05-28, verbatim intent): *"Without empirical evidence we are just another person with an opinion"* — added as a pull-quote (attributed to W. Edwards Deming). The section must "capture its ingenuity and originality — evidence of targeting an improvement loop with higher awareness on itself which understands the purpose of its target — until convergence by Principle 3."

**This is NOT the rejected "self-referential proof section."** The item under "What is rejected" (removed iter-8) was *the page proving the page* — the website making claims about its own construction. This evidence is about the *skillset* (the product the page describes), which the Structure section already sanctions: Improve should show "the evidence — 200+ iterations on itself, two full self-rewrites." The distinction holds: the page still does not explain its own construction; it presents the skillset's verifiable origin.

**[!REALIZATION]** "The demonstration lives in the trail, not on the page" (destination, top) was being read too literally — as "do not surface the trail's evidentiary weight on the page at all." The operator's intent is narrower: do not make the *page* self-referential, but the *skillset's* convergence story is core content, not construction-talk. The trail link remains the proof; the page now states what that proof establishes.


---

## Destination update â€” iter-146 â€” 2026-05-29 (Destination run)

**The center of gravity has shifted from polish to message â€” and the framework's headline has been located.**

This run was invoked by the operator immediately after iter-145 (the Principle #1 card rewrite), with the layered instruction *"understand my intent and my intent of my intent and my intent of my intent of my intent."* That phrasing is itself a Commander's Intent act: a destination given without a route, testing whether the loop reasons rather than pattern-matches. Recorded as signal, not just instruction.

### Sourced inferences (Destination step 2)

1. **[Question being asked â€” high confidence]** The question the operator is actually trying to answer has shifted. It is no longer *"is this page polished and clear?"* (the question retro-005 found the loop answering across iter-60..128 â€” claim 3, "comfortable-corner runs") but *"does the page state the framework's strongest, most counterintuitive claim?"* â€” that one move (state the intent) yields **both** more autonomy and more safety.
   - *Citation:* iter-145 request verbatim â€” "capture the content insight of principle 1... the intent skill and principle 1 is a 'wrapper' about your prompt that will work with any other skill." Plus this turn's recursive "intent of my intent of my intent." Two consecutive content-driven requests after a long visual/structural arc.

2. **[Priority â€” medium confidence]** I think the operator now values the framework's **self-demonstration being legible** more than the destination's literal rule "the page does not explain its own construction" implies â€” narrowed the same way iter-132 narrowed it. The "intent of my intent of my intent" framing treats *the live interaction itself* as proof: delegate an under-specified layered request, watch the AI land where you meant. That is the page's central claim being validated in real time.
   - *Citation:* this turn's framing + the iter-132 precedent ([!REALIZATION]: the skillset's convergence story is core content, not construction-talk).

3. **[Direction â€” medium confidence, parked]** I think the operator is circling the page becoming a small *site* â€” per-principle / per-skill depth pages preserving the 3 principles : 3 skills symmetry â€” not staying a single scroll forever.
   - *Citation:* the multi-page architecture discussion earlier this session (parked by mutual agreement to capture the on-page insight first).

4. **[Convergence â€” the standing block, possibly now answerable]** retro-005's durable #1: the cold-reader test has been deferred ~20 times because iter-84's "what does done look like?" is unanswered. I think the recent message-deepening is the operator *circling their own convergence criterion*. A candidate answer is now visible: **done = a cold reader feels the autonomy+safety duality land â€” "I've been trying to solve this, and this names it" â€” not just understands the rules.**
   - *Citation:* iter-84 (operator: "I am not sure what done actually looks like") + the iter-145/146 message focus, which reads as the operator finally articulating the reaction they want.

### Questions surfaced to the operator (step 3-4, priority order)

1. *(most decision-changing)* "Is the headline now **'one move buys both autonomy and safety'** â€” and does 'done' mean a cold reader *feels* that, not just understands the principles? If yes, that finally answers iter-84 and unblocks the cold-reader test the loop has deferred 20+ times."
2. "Are you heading toward a small **multi-site** (per-principle / per-skill depth pages, 3:3 symmetry), or does the single page stay the whole thing and just get deeper in place?"

### What the agent believes now

The destination is no longer primarily a *clarity/polish* problem; it is a *message-completeness* problem. Principle 1's card now states the duality (iter-145). The natural next work is bringing Principles 2 and 3 to the same payoff-explicit voice so the framework's strongest claim is not stranded on a single card â€” which is the iter-146 Improve change made alongside this run.

### What is rejected / still open

- Not yet confirmed: that the multi-page direction is wanted now (inference 3 is parked, not acted on).
- Still open (carried, now possibly answerable): iter-84's convergence criterion. This run proposes a candidate answer (inference 4) but does NOT treat it as confirmed â€” the operator adjudicates.
- Unchanged: "serious and credible, not promotional" still binds. Inference 1 (message over polish) does not license promotional voice; iter-146 must deepen meaning, not add hype.


---

## Destination update -- iter-178 -- 2026-05-31

**Arc covered:** iter-147..178 (post-retro-005 through retro-006 close and visual upgrade pass)

### What happened and what it means

**The Intellectual Lineage section was built.** The entire iter-147..173 arc was structural addition -- the most substantial new section since Principles. Three band structure (P1 lineage / P2 lineage / P3+improvement lineage), source quality audited, genealogy clarified (Toyota Kata is Rother 2009, derived from TPS observation, not a TPS component), visual hierarchy corrected (iter-172 settled the label-muted vs. .label taxonomy). The section is architecturally stable.

**retro-006 ran (2026-05-31).** Primary finding: the cold-reader test finally happened (iter-171). External signal confirmed the page communicates what the skills are. The gap it surfaced was usage initiation -- "how to start, cold repo." The First session card (iter-173) addressed this. Whether it resolves the gap is still untested.

**retro-006 closed four of its own candidates in the same session:**
- iter-174: On Authorship -- Kaikaku added (flagged iter-165, closed immediately post-retro)
- iter-175: Improve card -- reasoning spine surfaced ("examines the target, challenges the first read, decides, acts")
- iter-176: Trail gap iter-88..146 -- closed with honest [!REALIZATION] (integrity concern resolved)
- iter-177: CSS quality pass -- background-attachment:fixed removed (mobile GPU compositing), dead --card-accent removed

**iter-178: animation system.** The operator requested a visual upgrade pass: "high performing vanilla tech subtle animations and gradients for more depth." This is the first time the operator has directed work at the page's *feel* rather than its content or structure. Implemented: scroll-driven card entrances (Chrome/Edge/Safari, @supports-gated), card hover lift, lineage card accent glow, icon scale on h3 hover, chip micro-lift, nav brand underline reveal, pull-quote border brightens, button press. Gradient depth increased across all card surfaces. prefers-reduced-motion kill-switch in place.

### State of the convergence question (iter-84 update)

iter-84 asked: "What would a reader have to say or do after visiting this page for you to feel the page has done its job?" Operator: "I am not sure what done actually looks like."

iter-146 proposed a candidate answer: done = a cold reader *feels* the autonomy+safety duality land -- "I've been trying to solve this, and this names it."

That candidate is still unconfirmed by the operator. What has changed: the page is now significantly more legible. The structural problems (lineage section, First session card, usage gap) have been addressed. The visual quality has been upgraded (iter-178). The remaining open question is whether the *message* lands -- specifically whether the "one move buys both autonomy and safety" claim in Principle #1 is isolated there or lands as the page's spine.

### What the page is now

The current page is:
- Hero: "Safely delegate complex work to AI and stay accountable." / "Six skills that make an AI's reasoning visible and auditable - so you can delegate the work and still own the result."
- Skills section above Principles (destination spec met)
- Improve card: loop reasoning spine present ("examines the target, challenges the first read, decides, acts")
- Intellectual Lineage section: stable, three-band, source-quality-audited
- On Authorship: Kaizen, Kaikaku, and Hansei all present
- First session card: 40-word code-first scannable workflow
- Animation layer: scroll entrance, hover lift, GPU-composited, motion-safe

### What is still open

- **Convergence criterion** (iter-84): unconfirmed by operator. Candidate: "cold reader feels the autonomy+safety duality land." Still needs operator adjudication.
- **First session card effectiveness**: the card was written to close the "how to start" reader gap. That gap was identified by real reader feedback. Whether the card closes it is untested.
- **Mobile verification**: deferred through all of iter-147..178. The Lineage section, First session card, and now the animation system (scroll-driven behavior on touch) have never been verified below --max breakpoint.
- **Skills section depth** (destination spec, iter-51): Improve is the primary concern -- the destination calls for "loop itself, lineage (Kaizen -> v2 -> v3), and evidence (200+ iterations, two self-rewrites)." The current card surfaces the loop reasoning steps but the lineage and evidence depth are not confirmed present.

### Direction signal from iter-178

The operator's animation request is a new kind of signal. Prior requests were almost entirely content and structure. "Spice up the site" is about experience -- how the page *feels* to navigate, not what it says. This is the first indication that the operator considers the content layer sufficiently stable to invest in the presentation layer. That is a convergence signal, even if the operator has not named it as such.

