# Vision — pea-website

*Written by agent after Vision run, 2026-05-26. Operator commits when it reads right.*

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
- Feel that the work is **serious and credible**, not promotional

The current page fails this test. The hero leads with pain (the problem, at length) before the relief. The design relies on the text being read rather than the structure being seen. This is the primary open problem.

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

## Colour system (settled — session-007/008, updated iter-11)

**Light, not dark.** The Monokai dark palette (iter-4 through iter-6) was explicitly rejected.

**Palette:**
- `--bg: #fafaf8` — warm white
- `--ink: #1c1c1e` — near-black, ~17:1 contrast
- `--muted: #44403c` — warm stone grey, ~8:1 contrast (darkened from #57534e in iter-11)
- `--rule: #e7e5e4` — warm stone border
- `--accent: #155e75` — deep teal, ~7.2:1 contrast; bridges technical and non-technical audiences
- `--accent-lt: #f0fdfa` — pale teal tint (also used for inline code backgrounds)
- `--card-bg: #f5f5f3` — slightly elevated surface

---

## What is still open

- **Copy and visual hierarchy** — primary open problem. The hero leads with pain before relief. The design relies on text being read, not structure being seen. A non-technical reader does not get instant clarity. This is what is blocking publication.
- Browser visual check — first real render of the light theme still not done
- Push to remote / GitHub Pages — blocked by the copy/clarity problem above
