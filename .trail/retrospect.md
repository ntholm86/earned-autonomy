# retrospect.md — pea-website

_Last updated: 2026-05-27 (run: retro-002)_

---

## Freshness check

No `tools/record.py` exists in this repo — no derived artifact pipeline. `history.md` and `learning.md` are not present. Arc-claims derived directly from full read of `.trail/audit-trail.md` (1798 lines, sessions 001–039) and `.trail/vision.md` (post iter-39 update).

- `python tools/record.py history --write` — NOT AVAILABLE
- `python tools/record.py learning --write` — NOT AVAILABLE
- Gate: PASS (direct trail read; no stale derived artifacts to refresh)

---

## Current claims

**1. The design system has been rebuilt three times without an emotional destination — and all three were genuine improvements anyway.**

iter-7 (inline style removal), iter-33/34 (typography tokens + Kaikaku CSS), iter-36/38 (dark theme + semantic type colours). Each produced a clean, falsifiable diff and each closed a real gap. But none was grounded in what the page should make the reader *feel*. The emotional destination — "recognition + intrigue, I've been looking for this to safely delegate work to AI" — was named for the first time in iter-39. This means every prior design decision was made against structural criteria (contrast ratios, semantic clarity, token architecture) while the emotional register was implicit. The three rebuilds were necessary. A fourth should not be needed: the architecture is sound, the palette is confirmed, and the destination is now in vision.md.

**2. retro-001's "copy is the primary problem" was correct but incomplete — the copy problem has since been split in two, and one half remains open.**

retro-001 named structural clarity as the gap: hero leads with pain before relief, structure relies on text being read. iter-12–15 addressed this: answer-first hero, scannable taglines, de-jargon, three prose passes. The structural clarity problem is closed. What remains is *emotional* clarity: the reader should feel *found* in three seconds, not just informed. This is harder to verify from inside the loop — it requires a reader who has the problem. The loop has not tested the page against an actual non-technical reader at any point in 39 iterations.

**3. The CSS architecture investment (iter-7, iter-33, iter-34) is the most structurally stable part of the page and should not be touched.**

iter-7 made the palette reversal a 2-edit operation. iter-34's Kaikaku reduced CSS from ~800 to 327 lines and class names from ~50 to ~20. iter-38's semantic colour system required only 15 targeted swaps. The token architecture has paid off at every reversal point. No structural debt remains. Future agents should work within this system, not against it.

**4. vision.md drifted for 24 iterations between iter-36 and iter-39 — Vision runs are the only mechanism that catches this, and they only run when the operator asks.**

Iter-36 flagged the dark/light contradiction with `[!REVERSAL]`. Vision.md was not updated. 24 iterations passed. During that window, any fresh agent reading vision.md would have treated dark as a drift to correct. Improve does not check vision consistency; Vision runs do. Vision should be triggered periodically, not only when the operator asks — specifically: if two consecutive design runs feel like correction rather than refinement, trigger Vision before the third.

**5. The operator's visual reactions have been the primary quality signal throughout, but almost none are in the trail.**

Retro-001 wrongly claimed the browser check had "never been done." The operator corrected that it was done continuously and informally. The dark theme, the colour corrections, all three design rebuilds were operator-initiated from visual inspection. The trail captures what the agent did; it does not capture what the operator saw. This makes arc-level visual quality claims structurally incomplete.

**6. The page is approaching its final structural state. The single remaining open problem is the hero's emotional register.**

All sections exist and are stable. The design system is settled. The copy has been de-AI'd three times. The only gap named in iter-39 Vision is that the hero doesn't make the reader feel *found*. This is a targeted change, not a systemic one.

**7. Three Vision-level reversals occurred in the arc; each was operator-initiated and correct. The pattern is: operator overrides stale Vision constraints correctly, but the agent delays updating vision.md.**

Proof section removed (iter-8), light to dark (iter-36), trail section as evidence added back (iter-16). All three were right calls. All three created vision.md drift that persisted until a Vision run corrected it. The agent's job is to flag the contradiction and update vision.md in the same iteration or the immediately following Vision run — not 24 iterations later.

---

## What the next runs should test

**Primary (blocking publication):**

1. **Hero emotional register.** The h1 reads: "A framework for safely delegating real work to AI — while remaining accountable for what gets done." Accurate, but may read as a description rather than a recognition. The target (vision.md, iter-39): the reader feels "I've been looking for this." Test: does the first screen make a non-technical reader who has been frustrated with AI delegation think "this is for me" — before reading any body copy? If not, the h1 and opening line need to move from description to recognition.

2. **Visual verification of the dark theme.** The entire dark canvas + five-hue semantic colour system has never been browser-checked. Contrast ratios for `--sage (#a3d6a7)` and `--lavender (#c4a7e7)` on `--bg (#1e2030)` are estimated, not measured. `.numeral-circle` (white text on sage) and `em` text (lavender on dark bg) are highest-risk. Mobile viewport untested.

3. **Push to GitHub Pages.** The terminal readiness test. The site is static, zero dependencies, deployment is trivial. After the hero and visual check are done, there is no remaining blocker.

**Secondary (informational, not blocking):**

4. **External cold-reader test.** The page has never been shown to an actual non-technical reader. Every quality assessment has been agent-generated or operator-confirmed. A single cold read by someone who fits the primary reader profile is the highest-information move available that the loop has never taken.

---

## Active operational rules

- **Never add inline `style=""` attributes.** They accumulate silently and require dedicated cleanup. If a CSS class doesn't exist, create one.
- **All CSS changes go through `:root` tokens.** The 2-edit reversal property is the architecture's payoff. Maintain it.
- **Before inventing a new CSS class, verify no existing class already serves the role.** The iter-34 Kaikaku collapsed 50 bespoke classes to 20 generic ones. Accreting bespoke classes is the failure mode that makes future Kaikaku necessary.
- **`git add <explicit paths>` — never `git add -A`.** Iter-33 swept an unintended deletion via `-A`.
- **Append trail files with `Add-Content -Encoding UTF8`. Never `Set-Content`, never `>` redirection.** Iter-37 produced 124 mojibake em-dashes via a `Set-Content`/`Get-Content -Raw` round-trip. Even targeted in-place edits using `Set-Content` corrupt UTF-8 multi-byte sequences in PowerShell 5.1.
- **vision.md updates must be timely.** When a `[!REVERSAL]` fires, vision.md should be updated in the same iteration or the immediately following Vision run. A 24-iteration drift (iter-36 to iter-39) is too long.
- **Trigger Vision when two consecutive design-direction corrections occur.** Iter-34 (Kaikaku), iter-36 (dark theme), iter-38 (colour semantics) were three consecutive large corrections. A Vision run after the second would have named the emotional destination before the third.

---

## Loop-effectiveness notes

The loop has been effective at structural work and ineffective at emotional work. Structural changes (CSS tokens, class taxonomies, link credibility) produce verifiable diffs. Emotional register changes require testing against a reader who has the problem.

The page has been structurally sound since iter-34. The remaining gap is in a dimension the loop cannot self-verify. The next highest-leverage move is external validation: a cold reader, or a GitHub Pages push that exposes the page to real traffic.

**Retro-001's core claim held across 29 more iterations:** "The loop is biased toward safe, verifiable work at the expense of high-leverage, harder-to-verify work." The form of that bias has shifted — in retro-001 it was CSS over copy; now it is copy over emotional register. The same structural dynamic, one level up.

