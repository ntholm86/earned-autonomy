# retrospect.md — pea-website

_Last updated: 2026-05-28 (run: retro-005)_

---

## Freshness check

No `tools/record.py` in this repo. Arc-claims read directly from `audit-trail.md` (285KB) and `destination.md`.

- `python tools/record.py history --write` — NOT AVAILABLE
- `python tools/record.py learning --write` — NOT AVAILABLE
- Note: `history.md`/`learning.md` (mtime 16:40) are stale relative to `audit-trail.md` (mtime 20:38); they predate iter-121..128. No derivation tool exists to refresh them. Arc-claims were formed from the primary `audit-trail.md`, not the stale derived artifacts.
- Gate: PASS (direct trail read; derived artifacts knowingly bypassed, not relied upon)

---

## Scope statement

First full arc-read since retro-004 (which covered through iter-59). Question: across iter-60..iter-128, has the loop been advancing the destination, or polishing findable surfaces while the destination-critical work stays deferred? Specifically: did the cold-reader test that retro-004 declared "overdue, deferral exhausted" ever execute?

---

## Current claims

**1. The cold-reader test has now been deferred ~20 consecutive times and still has not run. retro-004 declared the structural justification for deferral "exhausted" after iter-59. Fifteen-plus iterations later (iter-60..87, iter-121..128) it remains the standing #1 and remains unexecuted. This is the single most durable fact about the arc.**

It was first named at iter-29, ranked #1 or #2 in essentially every entry since, and explicitly called "the move, not a candidate" by retro-004. The page is live at https://ntholm86.github.io/earned-autonomy/. The loop has had every structural precondition to gather external reader signal for 60+ iterations and has not. The deferral is no longer *about* the page — it is the loop's defining blind spot.

**2. The reason the cold-reader test keeps being deferred is upstream of the page: there is no operator-confirmed convergence criterion. (destination, iter-84: the operator said "I am not sure what done actually looks like.")** Without a definition of done, the loop optimizes for what is *findable* — de-ai passes, link targets, tooltip copy, dash style, spacing — because those produce a visible change every run. The one thing that would resolve "are we done?" requires two inputs the loop cannot self-generate: an external reader's reaction, and the operator's own statement of the target reaction. Until iter-84's open question is answered, every iteration is exploration-phase polish, not convergence-phase work. This is the deeper claim retro-004 missed by framing the deferral as merely "overdue."

**3. The recent arc (iter-121..128) is a textbook comfortable-corner run, and the loop correctly diagnosed it mid-stream.** Citations (121) → in-page anchor wiring (122) → dash normalization (123) → cross-link targeting (124) → tooltip unification (125, 126) → lineage footers (127) → card spacing (128). iter-126 itself declared the link/tooltip finding-class "exhausted" and warned the next run not to keep polishing it; iter-127/128 then moved to adjacent lineage-section polish. Healthy self-awareness, but the trajectory confirms claims 1–2: the loop is doing findable work because destination-critical work is blocked on operator input.

**4. The loop is structurally honest — this is NOT a confabulation trail.** Reversal/realization density is healthy across the arc: iter-126 carries an explicit [!REVERSAL] of iter-125's "intentional variance" judgment; iter-128 honestly conceded its change was "technically correct, an aesthetic legibility call, not a bug"; iter-121 caught two of its own 404s in post-edit verification and logged them; predictions are stated before action and checked after. The trail records its own misses. Confabulation is not the failure mode here — selective attention is.

**5. A second perpetually-deferred task mirrors the cold-reader pattern at smaller scale: the iter-88..iter-120 trail gap (33 iterations not logged).** Flagged as a Candidate Next Move in every entry from iter-121 through iter-128, never acted on. The loop now has two known-needed tasks it keeps ranking and never executing. The pattern (rank #1/#3, defer, repeat) is the tell, not the specific task.

**6. iter-128 performed the first browser render verification since the dark theme (iter-36).** destination still lists "Visual verification not done" and "Mobile viewport untested" as open. iter-128 closed the desktop half (rendered #foundations, confirmed spacing visually) but explicitly left mobile/narrow-width unverified. Visual verification is now a demonstrated capability in this loop, not a theoretical one.

---

## What the next runs should test

**Immediate — and this time it is blocked on the operator, not the loop:**

1. **Resolve iter-84's open question, then run the cold-reader test.** The loop cannot generate either input. The operator must answer: "What would a reader have to say or do after visiting this page for you to feel it has done its job?" Until then, convergence cannot be declared and further polish iterations have sharply diminishing returns. This is the move; everything else is deferral.

2. **Formally close the iter-88..iter-120 trail gap.** Either backfill terse entries from the git log, or record one explicit [!REALIZATION] that those micro-iterations were intentionally not logged — so the gap is documented rather than silently carried as a perpetual candidate.

3. **Mobile/narrow-width visual check.** iter-128's named blind spot; destination's standing open item. Now cheap (browser render is demonstrated). The lineage cards went full-width with a 2rem gap — confirm that reads well below the --max breakpoint.

---

## Active operational rules

*(Rules 1–14 carried forward from retro-004; rules 15–18 added retro-005. All still apply unless struck.)*

1. **Never add inline `style=""` attributes.** If a CSS class doesn't exist, create one.
2. **All CSS changes go through `:root` tokens.** The 2-edit reversal property is the architecture's payoff.
3. **Before inventing a new CSS class, verify no existing class serves the role.** Accreting bespoke classes is the failure mode that forces future Kaikaku.
4. **`git add <explicit paths>` — never `git add -A`.** (iter-33 swept an unintended deletion.)
5. **Append trail files with `Add-Content -Encoding UTF8`. Never `Set-Content`, never `>` redirection.** (iter-37 produced 124 mojibake em-dashes; a Set-Content round-trip corrupted retrospect.md again in retro-005.) Write via a temp UTF-8 file, append with `Add-Content`, then grep for `â€` to confirm clean.
6. **destination.md updates must be timely** when a [!REVERSAL] fires.
7. **Trigger a Vision/Destination run when two consecutive design-direction corrections occur.**
8. **Skills section appears above Principles in scroll order.**
9. **Skill order: Intent (P1) → Trail (P2) → Improve (P3) → [tier-2 separator] → Destination → Retrospect → Probe.**
10. **Improve is an expanded subsection (~2× depth), not a card.**
11. **De-AI pattern 13 is active.** Cut difficulty-announcement frames from headings/opening sentences.
12. **Labels use `--amber`** (structural announcements). Lavender = conceptual emphasis. (Corrected iter-76.)
13. **Trail markers ([!DECISION], [!REALIZATION], [!REVERSAL]) use `--amber`/`--amber-lt`** — technical identifiers, not danger signals.
14. **Skill cards use `div.card` + title-as-link (h3 > a), not whole-card-as-link.**
15. **[retro-005] The link/tooltip standardization finding-class is EXHAUSTED** (declared iter-126, confirmed by the iter-127/128 drift to adjacent polish). Do not open further link-target or tooltip-copy iterations. In-page links target the specific card (`#principle-N`, `#arf`, `#probe`); standalone links carry role-consistent `data-tip`; inline-prose links carry none (forcing `display:inline-block` breaks wrapping); same URL → identical tooltip.
16. **[retro-005] The page is hyphen-only.** Em-dashes were removed wholesale in iter-123 by operator preference. New page content must use plain hyphens, never `—` or `&mdash;`. (Trail/retrospect files may still use em-dashes; the rule is page-scoped.)
17. **[retro-005] Spacing ladder is `--gap-xs/sm/md/lg`; stack classes are `.stack` (sm) and `.stack-lg` (lg).** `.stack-md` was renamed away in iter-128. When changing a token-driven value, rename the class rather than leaving a name/value mismatch.
18. **[retro-005] Browser render verification is available and expected for visual/layout changes.** iter-128 used the integrated browser to confirm a spacing change. Use it before committing layout-affecting edits; do not rely on source reasoning alone for "does it look right."

---

## Loop-effectiveness notes

The loop is effective at execution and honest in its record (claim 4), but its attention allocation is the problem (claims 1–3). Across 60+ iterations spanning two retrospects, the highest-ranked move has been gathering external reader signal, and it has never once executed — because it is the one move the loop structurally cannot perform alone, and the operator has not yet supplied the missing inputs (a convergence criterion, a reader).

The kind of finding this loop will structurally miss: anything that requires an input from outside the artifact. It will reliably find and fix every internal inconsistency, every AI-tell, every misaligned token — and it will reliably *not* discover whether the page actually lands with a cold reader, because that signal does not exist inside the file. retro-004 saw the symptom and called it "overdue." retro-005's correction: it is not overdue, it is *blocked* — and naming it as a backlog item the loop should "just do" has been the subtle error, because it lets the operator-dependent precondition stay invisible. The honest status is: **the page is in the exploration phase, the loop has done the findable exploration thoroughly, and convergence is gated on an operator decision that iter-84 surfaced and no run since has resolved.**
