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
