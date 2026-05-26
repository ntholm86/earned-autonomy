# Vision — pea-website

*Written by agent after Vision run, 2026-05-26. Operator commits when it reads right.*

---

## The destination

A single-page public website that is the credible intellectual face of the Principles of Earned Autonomy ecosystem — legible to someone arriving cold from GitHub or Zenodo, and equally useful as a link sent to someone with partial context.

It is not a product page. It is not a personal portfolio. It is an intellectual position made accessible.

**The page is also a demonstration artifact.** This website was built using the PEA skills suite — Vision, Intent, Trail — and that fact is surfaced on the page itself. The build process (this session, with a committed trail) becomes part of the product. "Built in about 5 minutes using these skills" is operational credibility: the same logic as the suite running on itself 200+ times. The page doesn't just describe the skills — it *is* evidence they work.

---

## Reader

**Dual audience — both must be served:**
- Someone who stumbled here from GitHub, Zenodo, or a search: needs to understand from scratch what the problem is, why it matters, and what PEA offers.
- Someone who has been sent here with context already: needs confirmation that the work is serious and a clear map to go deeper.

The page must work for both without talking down to the informed reader or losing the uninformed one.

---

## Structure

Three sections, in this order:

1. **The Principles** — Commander's Intent, Observable Autonomy, Convergence Is Silence. Not as a bullet list of definitions. As an explanation of *what problem each principle solves* and *why that problem matters* for anyone delegating real work to an AI. This is the intellectual core.

2. **The Skillset** — The six skills (Intent, Vision, Trail, Improve, Retrospect, Probe) as the concrete implementation of those principles. Show what they do and why they hang together. Not a feature matrix — a coherent picture of how the principles become practice.

3. **Self-referential proof** — A closing section (or integrated note) that states: this page was built using the skills suite, in about 5 minutes, with a committed audit trail. Link to the trail or the build session as evidence. The page itself is a field case.

The harness protocol is out of scope for now.

The two content sections are **not framed as a connected stack**. The principles stand on their own. The skills are their enactment — but a reader who only understands the principles has gotten value.

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

---

## Colour system (settled — session-007/008)

**Light, not dark.** The Monokai dark palette (iter-4 through iter-6) was explicitly rejected: too dark, not easy to read, not professional enough for the dual audience.

**Palette:** warm white + deep teal.
- `--bg: #fafaf8` — warm white, slightly off pure white
- `--ink: #1c1c1e` — near-black, ~17:1 contrast on bg
- `--muted: #57534e` — warm stone grey, ~6.4:1 contrast
- `--accent: #155e75` — deep teal, ~7.2:1 contrast; distinctive, credible, bridges technical and non-technical audiences
- `--card-bg: #f5f5f3` — slightly elevated surface

**Rationale confirmed by operator:** deep teal was chosen over forest green and warm amber because it reads credible and distinctive for the dual audience (non-technical thinkers + technical evaluators) without defaulting to corporate blue.

---

## What is still open

- Browser visual check — first render of the light theme
- `prefers-color-scheme` dark fallback — deferred; dark was rejected, not deferred
- Push to remote / GitHub Pages — not yet public
