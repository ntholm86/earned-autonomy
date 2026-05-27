# Vision — pea-website

*Written by agent after Vision run, 2026-05-26. Updated 2026-05-27 (iter-39 Vision run). Operator commits when it reads right.*

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

Two content sections (no self-referential proof section):

1. **The Principles** — Commander's Intent, Observable Autonomy, Convergence Is Silence. Not as a bullet list of definitions. As an explanation of *what problem each principle solves* and *why that problem matters* for anyone delegating real work to an AI. This is the intellectual core.

2. **The Skillset** — The six skills (Intent, Vision, Trail, Improve, Retrospect, Probe) as the concrete implementation of those principles. Not a feature matrix — a coherent picture of how the principles become practice.

The harness protocol is out of scope for now.

The two content sections are **not framed as a connected stack**. The principles stand on their own. The skills are their enactment — but a reader who only understands the principles has gotten value.

## What success looks like

A non-technical reader arriving cold should:
- Understand **what PEA is and what problem it solves** within 3 seconds — without reading
- Get the **point** of the three principles within 30 seconds — by scanning, not reading
- Feel **recognition + intrigue**: "I didn't know this existed, but now that I see it, I needed it" — not impressed, not informed, *found*

**Emotional destination (confirmed 2026-05-27):** the primary reader has been trying to safely delegate real work to AI, finds it hard to trust, and lands on this page feeling: *this names the thing I've been struggling with.*

"Serious and credible, not promotional" remains a valid constraint — but it describes how the page is *evaluated* after reading. The primary register to achieve is recognition in the first three seconds. Credibility is what makes the recognition stick.

The current page fails this test. The hero leads with pain before relief. The design relies on text being read rather than structure being seen. Operator confirmed 2026-05-27: *"it does not give this instant feeling of solving that hard problem."*

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
