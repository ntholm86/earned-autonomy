# retrospect.md — pea-website

_Last updated: 2026-05-27 (run: retro-003)_

---

## Freshness check

No `tools/record.py` in this repo. No `history.md` or `learning.md`. Arc-claims read directly from `audit-trail.md` (2435 lines, sessions 001–iter-51 Vision) and the newly updated `vision.md` (iter-51 skills-first shift).

- `python tools/record.py history --write` — NOT AVAILABLE
- `python tools/record.py learning --write` — NOT AVAILABLE
- Gate: PASS (direct trail read; no stale derived artifacts)

---

## Scope statement

Vision shifted in iter-51: the page inverts from framework-explanation (Principles first) to skills-adoption (Skills first). Read the full arc against the new direction and determine: what structural facts need changing, what operational rules need updating, where is the loop's attention needed now?

---

## Current claims

**1. The arc built a framework explanation page for 50 iterations. The page is now about to become a skills adoption page. This is the largest content-structure inversion since iter-34 Kaikaku — but it only touches section order and Improve depth, not CSS.**

Every content decision from session-001 onward was made under "Principles first, Skills as enactment." That directive reversed in the iter-51 Vision run. The sections already exist; what changes is: Skills moves above Principles in scroll order, skill card order changes to Trail → Intent → Improve → Vision → Retrospect → Probe, and Improve becomes a subsection rather than a card. The CSS architecture is not implicated — all tokens and utility classes remain valid.

**2. Improve has run 50+ times to build this page and still gets equal visual weight to Probe or Retrospect. That is the most significant content inconsistency in the current state.**

The page was built through Improve iterations. Improve is the loop itself, not a feature of the loop. The new vision names the fix: Improve gets ~2× depth, showing the loop steps (read trail → examine → challenge → decide → one change → verify → reflect), the lineage (Kaizen from Toyota Kata → v2 split into Kaizen/Kaikaku/Hansei → v3 unified), and the 200+ iteration evidence. A card that treats Improve like Vision or Probe understates what it is.

**3. Trail has been a showcase section since session-001 but has never been the recognition hook. Moving it to the first skill card is the application of the recognition insight from iter-39 that was applied to the hero but never applied to the skills ordering.**

Iter-39 named recognition as the primary register — "this names the thing I've been struggling with." Iter-40 applied that to the h1. The skills section was never reordered to match. The new vision corrects it: Trail first, because that is what developers realize they are missing.

**4. The external cold-reader test is the longest continuously deferred item in the arc. It has appeared in candidate-next-moves in 8 or more consecutive trail entries and has never been executed.**

First named in iter-43 cold audit. Listed as #1 or #2 in every subsequent trail entry through iter-50. The page is now publicly live at `https://ntholm86.github.io/earned-autonomy/`. The structural reorder about to happen will change the page before any cold reader sees it — correct sequencing. But after the reorder commits, this is the next move. Not the next candidate. The move.

**5. The page has 200+ Improve iterations of history and surfaces almost none of it. The build story — how the loop built itself, twice, over two rewrites — is the most credible proof of concept available and is invisible to the reader.**

Evidence section item 1 mentions "200+ iterations" in three sentences. The new vision names this as a fuller story belonging in the Improve section: two full self-rewrites, the Kaizen origin, the three-model convergence baseline. This is proof of concept for the framework, built by the framework.

**6. Vision drift prevention is working. The iter-51 Vision run fired in the same session that named the structural shift — the fastest vision-response in the arc.**

The 24-iteration drift of iter-36 → iter-39 was the named failure. Iter-51 corrected a structural direction change in the same session it was named. The operational rule from retro-002 is holding.

**7. retro-002's claim "page is approaching final structural state" is now superseded. It was accurate under the old vision. The new vision opens a structural iteration: section order, Improve depth, skill hierarchy.**

Retro-002 claim 6 should not be read as a constraint against the current direction. The CSS is stable. The content structure is not — intentionally, by operator direction.

---

## What the next runs should test

**Immediate (structural reorder — the active work):**

1. **Move Skills section above Principles.** Skills becomes section 2 (after hero); Principles moves to section 3. Navigation labels update to reflect new order.

2. **Reorder skill cards: Trail → Intent → Improve → Vision → Retrospect → Probe.** Trail leads.

3. **Expand Improve to a subsection with ~2× visual depth.** Show: (a) the loop steps in scannable form, (b) Kaizen/Toyota Kata lineage, (c) the 200+ iteration evidence (two self-rewrites, three-model convergence). Not a card.

4. **Reframe Principles section header.** Position it as intellectual grounding beneath the skills — "why the skills are built this way" — not the entry point.

**After the reorder:**

5. **Cold-reader test — execute it.** Not a candidate. The move. The page will be publicly live and structurally settled. This is the only quality signal the loop cannot generate itself.

6. **Confirm placement of "Delegate to AI. Own the work."** Formed in Vision iter-51. Tightest compression of the page's core message in the arc. Where it lives on the page is still open.

---

## Active operational rules

*(Rules 1–7 from retro-002; rules 8–11 added retro-003)*

1. **Never add inline `style=""` attributes.** They accumulate silently and require dedicated cleanup. If a CSS class doesn't exist, create one.

2. **All CSS changes go through `:root` tokens.** The 2-edit reversal property is the architecture's payoff. Maintain it.

3. **Before inventing a new CSS class, verify no existing class already serves the role.** The iter-34 Kaikaku collapsed ~50 bespoke classes to ~20. Accreting bespoke classes is the failure mode that makes future Kaikaku necessary.

4. **`git add <explicit paths>` — never `git add -A`.** Iter-33 swept an unintended deletion via `-A`.

5. **Append trail files with `Add-Content -Encoding UTF8`. Never `Set-Content`, never `>` redirection.** Iter-37 produced 124 mojibake em-dashes via a `Set-Content`/`Get-Content -Raw` round-trip.

6. **vision.md updates must be timely.** When a `[!REVERSAL]` fires, vision.md should be updated in the same iteration or the immediately following Vision run.

7. **Trigger Vision when two consecutive design-direction corrections occur.** Prevented the 24-iteration drift from recurring.

8. **Skills section appears above Principles in scroll order.** Per Vision iter-51. Vision constraint, not a candidate.

9. **Skill card order: Trail → Intent → Improve → Vision → Retrospect → Probe.** Per Vision iter-51.

10. **Improve is not a card — it is an expanded subsection with ~2× visual depth.** Must show: the loop steps, the Kaizen/Toyota Kata lineage, the 200+ iteration evidence. Do not compress to card format.

11. **De-AI pattern 13 is now active.** Check all headings and opening sentences for difficulty-announcement frames: "The hard part is...", "The tricky part is...", "The key challenge is...". Cut the frame; say the claim.

---

## Loop-effectiveness notes

The loop has been effective at structural work and has consistently deferred the highest-uncertainty move (cold-reader test). That deferral was defensible while the page was unstable. It is no longer defensible after the structural reorder completes.

**Retro-001 and retro-002 identified the same structural dynamic:** the loop is biased toward safe, verifiable changes at the expense of high-leverage, harder-to-verify ones. External validation is the only thing the loop structurally cannot provide for itself — which is exactly why it keeps being deferred. After the reorder: external.


