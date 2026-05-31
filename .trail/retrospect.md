# retrospect.md — pea-website

_Last updated: 2026-05-31 (run: retro-006)_

---

## Freshness check

No 	ools/record.py in this repo. Arc-claims read directly from udit-trail.md (62 entries) and destination.md. history.md/learning.md are stale derived artifacts; arc-claims formed from the primary trail.

- Gate: PASS (direct trail read; derived artifacts not relied upon)

---

## Scope statement

Read the arc from retro-005's close (covering through iter-128) to the current state (iter-173). Central question: Did the operator-gate unblock? Specifically - did the cold-reader test execute, and what did the arc do with the result?

---

## Current claims

**1. The cold-reader test finally ran. retro-005's central concern is resolved.**

After 20+ consecutive deferrals, the operator gathered real external reader signal. Verbatim feedback (iter-171): readers find installing the skills easy; "understanding how to exactly use them is harder" - specifically how to start, when to invoke each skill, cold repo with no .trail/. This is the first external reader signal since the page launched. retro-005 diagnosed the situation as "blocked on operator input"; that block has now lifted.

**2. The page's gap has moved from "intellectual clarity" to "usage initiation."**

The cold-reader signal shows the page successfully communicates what the skills are. The standing gap is the temporal workflow: what first, what next. Install closes the technical gap; skill cards close the conceptual gap; the bridge between them was absent. iters 171/173 addressed this with the "First session" card - a 40-word, code-first scannable workflow that answers three specific questions: cold repo start, skill sequence, session-to-session rhythm. The card was iterated twice (110 words -> 40 words, iter-173) before it reached a scannable format. The reader-gap is now addressed on the page; whether it is resolved is still untested.

**3. The Intellectual Lineage section is architecturally stable with one known open item.**

The section was built across the recent arc (~iter-147..173) - the most substantial structural addition since the Principles section. Source quality was audited (iter-168), genealogy clarified (iter-169: Toyota Kata is Rother's 2009 teaching framework derived from TPS observation, not a TPS component), cards ordered into three clean bands (iter-170: P1 / P2 / P3+improvement), visual hierarchy corrected (iter-172). One known open item remains: the "On Authorship" card reads "Kaizen and Hansei are post-war Japanese manufacturing" - Kaikaku was named on the page in iter-166 but is still missing from that sentence. Flagged iter-165, still unresolved.

**4. The label taxonomy ambiguity is resolved and has system-wide implications.**

iter-172 produced a [!REALIZATION] with permanent value: label-muted = organizer/category (sits above multiple items, groups them); .label (teal default) = content-header (primary anchor inside a content block). The TPS card triggered this because it is the only card with internal sub-sections. The distinction was implicit before iter-172; it is now explicit. Any future card with internal sub-sections must follow this rule.

**5. The iter-88..iter-146 trail gap (58+ iterations) remains undocumented and is now an integrity concern.**

retro-005 flagged iter-88..iter-120 as a 33-iteration gap, ranked it candidate next move #2, and it still was not resolved. The gap has grown: the trail jumps from iter-87 to iter-147 with no entries for any iteration in between - 59 iterations. The audit trail is the verifiable record of Observable Autonomy. An undocumented 59-iteration gap that survives three retrospect cycles is no longer just a deferred task - it undermines the arc's own claim to being an auditable record. The longer this stays open, the harder a backfill becomes.

**6. Mobile visual verification has been available since iter-128 and has never been used.**

retro-005 declared it "now cheap (browser render is demonstrated)" and named it candidate next move #3. iter-129..173 produced no mobile check. The Lineage section (iter-147..173) introduced new HTML layouts (.lineage-card, .tps-practice sub-sections, .lineage-title, .lineage-meta) that have never been verified below the --max breakpoint. Live readers have been using the page during this period.

**7. The skills section (destination's primary content) received no direct attention across iter-147..173.**

The entire recent arc was Intellectual Lineage. The destination (iter-51) specifies that Improve should show the loop itself, the lineage (Kaizen -> Kaizen/Kaikaku/Hansei -> unified), and evidence (200+ iterations, two full self-rewrites). iter-80 removed Lineage and Evidence from the Improve card. It is not recorded that this was ever reversed or supplemented. If the destination spec for Improve is still unmet, the section has been unchanged for 90+ iterations while the arc was working around it.

---

## What the next runs should test

**1. "On Authorship" Kaikaku fix - one sentence, flagged iter-165, never closed.**
Embarrassingly small. Do it first. The sentence currently reads "Kaizen and Hansei are post-war Japanese manufacturing." - add Kaikaku.

**2. Mobile visual check - Lineage cards and First session card.**
.lineage-card, .tps-practice, and the new "First session" .card are all unverified below --max. Browser render is a demonstrated capability. Do it before adding more content to the Lineage section.

**3. Formally close the iter-88..iter-146 trail gap.**
Backfill terse entries from the git log, or append one explicit [!REALIZATION] documenting that those micro-iterations were intentionally not logged. Either action closes the integrity concern. Continued deferral is not acceptable - the gap now spans 59 iterations across three retrospect cycles.

**4. Verify Improve card against its destination spec (iter-51).**
Destination says Improve should show: the loop itself (read -> examine -> challenge -> decide -> one change -> verify -> reflect), the lineage (Kaizen -> v2 -> v3 unified), and evidence (200+ iterations, two self-rewrites). Read the current Improve card and confirm whether this spec is met or whether iter-80 left it partially gutted.

**5. Confirm the First session card closes the reader gap.**
Operator-reported gap: "how to exactly use them." The iter-173 card answers "what first, what next." The remaining question is whether "when to invoke each skill during a live session" is also answered, or whether a second pass is needed. The test is whether a reader who was previously stuck can now self-unblock.

---

## Active operational rules

*(Rules 1-18 carried forward from retro-005; rules 19-20 added retro-006.)*

1. Never add inline style="" attributes. If a CSS class doesn't exist, create one.
2. All CSS changes go through :root tokens.
3. Before inventing a new CSS class, verify no existing class serves the role.
4. git add <explicit paths> - never git add -A.
5. Append trail files with Add-Content -Encoding UTF8. Never Set-Content, never > redirection. Write via a temp UTF-8 file, append with Add-Content, then grep for e to confirm clean.
6. destination.md updates must be timely when a [!REVERSAL] fires.
7. Trigger a Vision/Destination run when two consecutive design-direction corrections occur.
8. Skills section appears above Principles in scroll order.
9. Skill order: Intent (P1) -> Trail (P2) -> Improve (P3) -> [tier-2 separator] -> Destination -> Retrospect -> Probe.
10. Improve is an expanded subsection (~2x depth), not a card.
11. De-AI pattern 13 is active. Cut difficulty-announcement frames from headings/opening sentences.
12. Labels use --amber (structural announcements). Lavender = conceptual emphasis.
13. Trail markers ([!DECISION], [!REALIZATION], [!REVERSAL]) use --amber/--amber-lt.
14. Skill cards use div.card + title-as-link (h3 > a), not whole-card-as-link.
15. The link/tooltip standardization finding-class is EXHAUSTED (declared iter-126). Do not open further link-target or tooltip-copy iterations.
16. The page is hyphen-only. Em-dashes were removed wholesale in iter-123. New page content uses plain hyphens, never -- or &mdash;. (Trail/retrospect files may use em-dashes; rule is page-scoped.)
17. Spacing ladder is --gap-xs/sm/md/lg; stack classes are .stack (sm) and .stack-lg (lg).
18. Browser render verification is available and expected for visual/layout changes. Use it before committing layout-affecting edits.
19. [retro-006] label-muted = organizer/category label (sits above multiple items, groups them). .label (teal default) = content-header (primary anchor inside a content block). The TPS card is the canonical example: KAIZEN/KAIKAKU/HANSEI are .label; "Conceptual traditions" above the whole section is .label-muted.
20. [retro-006] The "On Authorship" sentence pattern ("X and Y are post-war Japanese manufacturing") must include all three TPS concepts when Kaikaku is referenced elsewhere on the page. The sentence currently omits Kaikaku - fix it before adding any further Lineage content.

---

## Loop-effectiveness notes

The most significant arc-level change since retro-005: the operator-gate unblocked. The loop's defining blind spot (cold-reader signal never gathered) is resolved at the input level. The response was structurally correct - real feedback, real gap identified, addressed in two iterations. This is the loop working as designed.

The remaining effectiveness concern is the iter-88..iter-146 gap. Observable Autonomy is the page's stated subject. Carrying a 59-iteration undocumented gap in the page's own audit trail for three retrospect cycles is a credibility problem, not just a housekeeping task. The loop has demonstrated it can prioritize closing gaps (iter-172 closed the label ambiguity gap immediately on discovery). It has also demonstrated it can defer indefinitely when a gap requires retrospection rather than a file edit. The trail gap requires retrospection. That is the pattern.
