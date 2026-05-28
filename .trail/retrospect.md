# retrospect.md — pea-website

_Last updated: 2026-05-28 (run: retro-004)_

---

## Freshness check

No 	ools/record.py in this repo. Arc-claims read directly from udit-trail.md (212KB, sessions 001–iter-59) and the updated ision.md (iter-59 vision update appended).

- python tools/record.py history --write — NOT AVAILABLE
- python tools/record.py learning --write — NOT AVAILABLE
- Gate: PASS (direct trail read; no stale derived artifacts)

---

## Scope statement

Vision was updated in iter-59 (skills section Kaikaku: principle framing, two-tier structure, label color change, card interaction pattern change). Read the full arc against the new vision and determine: what structural facts need updating, which operational rules changed, where is the loop's attention needed now.

---

## Current claims

**1. The arc has now gone through two major structural inversions in the same week. The page is no longer a framework-explanation site — it is a skills-adoption site with principle grounding. This is the correct destination.**

Session-001 through iter-50 built a principles-first page under the original vision. Iter-51-52 inverted the section order (skills above principles). Iter-59 went further: the skills section now maps each tier-1 skill to its principle (P1→Intent, P2→Trail, P3→Improve), names the tier-2 group as memory/reasoning/self-reflection, and removes the whole-card-as-link pattern. The destination is now clear in the artifact, not just in vision.md.

**2. The cold-reader test has been the #1 ranked next move in 12+ consecutive trail entries and has never been executed. After iter-59, the structure is the most settled it has been in the arc. The case for deferral is gone.**

First named at iter-29 (blind spot). Cited as #1 or #2 in every candidate-next-moves section through iter-59. Each deferral was defended on the grounds of structural instability — the page kept changing. After iter-59: the skills section framing is settled, the two-tier structure is in place, the color system is consistent, the principles-below-skills order is confirmed. The page is live at https://ntholm86.github.io/earned-autonomy/. There is no remaining structural defense for deferral.

**3. The color system has been revised three times: light→dark (iter-36), and now coral→lavender for labels + coral→amber for trail markers (iter-59). Each revision was correct. The system is now semantically cleaner.**

Prior semantic assignment: coral = structural announcements (labels, trail markers). That mapped a warning color to navigation elements, creating ambient danger signaling. Current assignment: lavender = conceptual emphasis (labels), mber = technical identifiers (trail markers, code). Coral now has no UI role except as a brand color in nav. This is the most semantically coherent the color system has been.

**4. The principle-to-skill framing (P1=Intent, P2=Trail, P3=Improve) is the highest-leverage content addition in the arc. It was always implied but never surfaced. Iter-59 made it explicit.**

The skills suite was built to enact the three principles. The page never said which skill enacts which principle. A reader landing on the skills section had no reason to connect Intent to Commander's Intent or Trail to Observable Autonomy. The label now makes that connection on first glance. This is the argument the page was always making — iter-59 said it out loud.

**5. The loop has been running de-ai passes reactively (when the operator notices a tell) rather than systematically. Two de-ai skill updates were made this session: pattern 9 (spatial-void) and pattern 3 sub-class (em-dash connector). Both were triggered by operator feedback, not by the loop proactively running the skill.**

This is not a failure — the operator catching tells is the skill working. But a systematic de-ai pass (running all 13 patterns against the full page) has never been done as a standalone iteration. One was attempted this session and produced four gap-removal edits (iter-57). The precedent is there.

**6. The two-tier skill structure (tier-1: immediate-use; tier-2: memory/reasoning) is new and unvalidated. It is the right conceptual frame — the operator confirmed it. It has not been seen by a reader who didn't already know the framework.**

The two-tier label ("Memory, reasoning & self-reflection") above Vision/Retrospect/Probe is new as of iter-59. It accurately describes when those skills become useful. A cold reader seeing it for the first time may or may not read it that way. Only the cold-reader test resolves this.

---

## What the next runs should test

**Immediate:**

1. **Cold-reader test.** Not a candidate. The move. The page is structurally settled, live, and the deferral justification is exhausted. This is the only signal the loop cannot generate for itself. After 12+ deferrals, executing it is overdue.

2. **Validate tier-2 label copy.** "Memory, reasoning & self-reflection" — does a cold reader understand what this tier is for? This is the only new content element in iter-59 that carries real semantic risk. The cold-reader test will surface this.

3. **Hero card block — de-ai pass.** The hero card ("Two responses are common...") was not touched in iter-57 or iter-58. It has not received a systematic de-ai pass. It is the first substantive prose a reader encounters after the h1.

---

## Active operational rules

*(Rules 1–7 from retro-002; rules 8–13 from retro-003/iter-59)*

1. **Never add inline style="" attributes.** They accumulate silently and require dedicated cleanup. If a CSS class doesn't exist, create one.

2. **All CSS changes go through :root tokens.** The 2-edit reversal property is the architecture's payoff. Maintain it.

3. **Before inventing a new CSS class, verify no existing class already serves the role.** The iter-34 Kaikaku collapsed ~50 bespoke classes to ~20. Accreting bespoke classes is the failure mode that makes future Kaikaku necessary.

4. **git add <explicit paths> — never git add -A.** Iter-33 swept an unintended deletion via -A.

5. **Append trail files with Add-Content -Encoding UTF8. Never Set-Content, never > redirection.** Iter-37 produced 124 mojibake em-dashes via a Set-Content/Get-Content -Raw round-trip.

6. **vision.md updates must be timely.** When a [!REVERSAL] fires, vision.md should be updated in the same iteration or the immediately following Vision run.

7. **Trigger Vision when two consecutive design-direction corrections occur.** Prevented the 24-iteration drift from recurring.

8. **Skills section appears above Principles in scroll order.** Per Vision iter-51.

9. **[REVISED iter-59] Skill order: Intent (P1) → Trail (P2) → Improve (P3) → [tier-2 separator] → Vision → Retrospect → Probe.** Supersedes retro-003 rule 9 (Trail→Intent). Principle order (P1→P2→P3) is the correct ordering.

10. **Improve is not a card — it is an expanded subsection with ~2× visual depth.** Must show: the loop steps, the Kaizen/Toyota Kata lineage, the 200+ iteration evidence. Do not compress to card format.

11. **De-AI pattern 13 is active.** Check all headings and opening sentences for difficulty-announcement frames. Cut the frame; say the claim.

12. **Labels use --lavender, not --coral.** Coral on navigation/label elements communicates danger. Lavender = conceptual emphasis. [Added iter-59]

13. **Trail markers ([!DECISION], [!REALIZATION], [!REVERSAL]) use --amber / --amber-lt.** These are technical identifiers, not danger signals. [Added iter-59]

14. **Skill cards use div.card + title-as-link (h3 > a), not .card.** Whole-card-as-link was inconsistent with Improve (which can never be an anchor). Title-as-link is the normalized pattern. [Added iter-59]

---

## Loop-effectiveness notes

The loop is effective and structurally honest. The [!REVERSAL] count is healthy (7+ confirmed reversals across the arc) — this is not a confabulation loop. The most significant finding is the sustained cold-reader deferral: 12+ consecutive entries, always ranked #1, never executed. That pattern is the clearest signal the loop has about where its own blind spot lies.

After iter-59, the structural work is done. What remains is validation — which only an external reader can provide.
