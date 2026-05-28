# Learning

Auto-generated from `.trail/audit-trail.md` by the `record.py learning --write` command in the autonomous-agent-skills install.
Do not edit by hand — re-run the command to refresh.

Compact chronological extract of every `[!REALIZATION]` and `[!REVERSAL]` marker. The learning surface — what the loop has actually concluded across runs. Read this before reading `audit-trail.md` in full; reach for `audit-trail.md` only when an item here needs its surrounding context.

## 2026-05-26 — session-005 — improve-iter-4 — Monokai dark colour scheme

**[!REALIZATION]** :* not fired — "~5 minutes" realization and lineage decisions are unaffected by a colour change.

## 2026-05-26 — session-008 — improve-iter-7 — light theme

**[!REALIZATION]** :** The iter-6 CSS architecture refactor (semantic variables, no inline styles) reduced what could have been a large cross-file change to exactly 2 edits. This is the concrete payoff of KISS/DRY — the architecture makes correctness tractable. A page that had inline `color: #66d9e8` scattered across the HTML would have required 20+ edits to re-theme.

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REALIZATION]** :** The 13 inline styles were not random — they all came from the same root cause: each session fixed a local visual need without asking "does a CSS class exist for this?" The correct discipline is: never write `style="..."` in the HTML body; if the property doesn't have a CSS class, create one. This session enforces that discipline structurally.

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REALIZATION]** :* not fired -- consistent with session-009 [!REALIZATION] ("next work is copy, not CSS").

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REALIZATION]** :* not fired.

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REALIZATION]** The h1 and the author voice are now in dialogue

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REALIZATION]** AI fingerprints are structural patterns, not word choices

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REVERSAL]** trail entry.** Session-1 Vision required self-referential proof. Iter-8 removed it. No individual trail entry marks this as a reversal. The Vision run (session-9) caught it retrospectively.

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REVERSAL]** on retro-001 arc-claim #4

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REVERSAL]** marker and corrected text. Claim #6 updated to remove browser check as an open item. Browser check removed from "What the next runs should test" and operational rules.

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REVERSAL]** Vision constraint overridden by operator

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REVERSAL]** : a Vision-level constraint was removed by operator direction, not by agent initiative.

## 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

**[!REVERSAL]** iter-17 author voice draft was wrong

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** same splice class appeared twice = pattern, convergence chain reset

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** When teaching a structure, the urge to simplify can quietly erase the distinctions that make the structure work. The four-file version felt cleaner and was easier to memorize, but it collapsed audit-trail.md and sessions/ into one concept - and that collapse is exactly what trail/SKILL.md warns against. The operator caught the omission immediately because they know the system. A reader who didn't know the system would have built an incorrect mental model from my page.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** The three-tier framing (operator / synthesis / evidence) was not in any single skill - it emerged from looking at all seven items at once and noticing the natural grouping (who writes, who derives, who appends). This is the kind of synthesis the page can offer that no individual skill document does. Future iterations should look for more cross-skill synthesis like this rather than just mirroring individual skills.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** The page's natural reading order is now a complete arc: principle -> mechanism (skills) -> what gets created (memory) -> how to use it (quickstart) -> what success looks like (trail). The trail section, which used to sit awkwardly after Memory Model, now has a clear role: it is the "after" picture for what the quickstart produces. Before this run, that section was floating. The new quickstart anchored it.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** The previous version's complexity came from a teacher's instinct - explain each step, gate each step, show every artefact. That instinct produces good written tutorials and bad landing-page sections. The landing page's job is to lower the barrier to trying it, not to teach the full procedure. The full procedure already exists at QUICKSTART.md; the page should defer to it, not duplicate it.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** The deai skill paid off most on the headline. "One real run in ten minutes" sounded reasonable in isolation but read as a sales pitch in context - I was selling rather than describing. "Three commands" is the smallest true sentence that does the same job. When a headline contains a quantity that the reader has to take on faith ("ten minutes"), that is almost always a sign the headline is selling. When the quantity is something the reader can verify by counting on the screen ("three"), the headline is describing.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** The operator caught two things in one request: (a) the explicit "CSS is messy" complaint, and (b) the implicit fact that I had quietly drifted from the established architecture by adding inline styles in three recent iterations. Inline-style debris is the exact failure mode retrospect.md warned about ("they accumulate silently across sessions"). The vision skill surfaced it - a normal Improve run would have just done the CSS refactor and missed the rule violation.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** :* not fired - iter-33 extends iter-7's tokenisation architecture rather than contradicting it.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REALIZATION]** ** The class redundancy was not designed â€” it accreted. iter-26 added section A, copy-pasted A's class names with a new prefix for section B in a later iter, did it again for section C. By the time the page had eight sections, "eyebrow" lived under nine different names. The token discipline established in iter-33 only reaches the values; it does not touch the *class taxonomy* that consumes those values. Tokenising values inside a duplicated class graph still leaves the duplication. Naming discipline is a separate axis from value discipline, and the recurring-class-debris pattern that retrospect.md called out across iter-26/28/30 is the visible signature of *that* discipline being absent.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REVERSAL]** Within-iteration scope broadening: `git add -A` swept a pre-existing deletion of `content/image.png` into the iter-33 commit. The file was orphaned (no grep hits anywhere in the repo) so the deletion is correct, but it was not in my stated scope. Lesson: when working in a repo with possible operator-side pending changes, use `git add <specific-files>` not `-A`. Recording this rather than silently passing it off.

## 2026-05-27 — iter-26 - trail-section-rebuild

**[!REVERSAL]** ` lesson). Commit `fc45ea3`: 424 insertions, 931 deletions.

## 2026-05-01 — iter-35-prose-simplification

**[!REALIZATION]** ** Once the design system carries weight, the prose can stop carrying that weight - and *should* stop, or it becomes redundant scaffolding. A tightened design system should always be followed by a prose pass.

## 2026-05-27 — iter-36-dark-theme-section-scoped-accents

**[!REALIZATION]** ** Section-scoped CSS custom properties via descendant selectors are a load-bearing tool for design systems. One --accent token + N section-scope rules outperforms N parallel token definitions on every dimension: smaller diff, no naming sprawl, automatic propagation to every dependent rule. This pattern should be the default whenever a single token must vary by region. Worth carrying forward.

## 2026-05-27 — iter-36-dark-theme-section-scoped-accents

**[!REALIZATION]** :* FIRED. This iteration contradicts the "Light, not dark" decision in vision.md (session-007/008 vintage). The contradiction is acknowledged in the [!REVERSAL] marker above and is by operator request, not autonomous drift. Already surfaced - no separate macro-reflection needed.

## 2026-05-27 — iter-36-dark-theme-section-scoped-accents

**[!REVERSAL]** Vision-contradicting move

## 2026-05-27 — iter-37-footer-de-ai-followup

**[!REALIZATION]** ** *Iter-35 missed the meta-frame because the agent was applying de-AI as muscle memory, not as a catalogued lens.* The pattern survived because it had no named home. Codifying the catalogue upstream is the structural fix. This is the **third consecutive iteration that touched prose tells** (iter-29 hedging audit, iter-35 simplification, iter-37 meta-frame). Three out of last seven is approaching pattern density - worth a Retrospect.

## 2026-05-27 — iter-37-footer-de-ai-followup

**[!REALIZATION]** :* not fired.

## 2026-05-27 — iter-38-semantic-colour-system

**[!REALIZATION]** :* MILD — iter-36's [!REALIZATION] celebrated section-scoped CSS custom properties as a "load-bearing tool for design systems." That was right as a *technique*; this iteration corrects the *axis* it was applied on (section geography vs. semantic type). The technique was sound; the application was wrong.

## 2026-05-27 — iter-43-cold-audit-p3-tagline

**[!REALIZATION]** : not fired — checked, no contradiction.

## 2026-05-27 — iter-44-hero-secondary-cta

**[!REALIZATION]** : not fired.

## 2026-05-27 — iter-45-get-started-nav

**[!REALIZATION]** : not fired.

## 2026-05-27 — iter-46-nav-order-get-started-before-trail

**[!REALIZATION]** : not fired.

## 2026-05-27 — iter-47-inline-style-cleanup

**[!REALIZATION]** ** The cleanup revealed 8 recurring patterns, not arbitrary one-offs. The most frequent (margin-top: var(--gap-md), 10 occurrences) and the evidence row pattern (align-items: flex-start + flex: 1, 3 occurrences each) suggest the original build did not have utility classes for common spacing and flex needs. The iter-34 Kaikaku addressed component classes; it left spacing utilities out. This pass fills that gap.

## 2026-05-27 — iter-47-inline-style-cleanup

**[!REALIZATION]** : not fired.

## 2026-05-27 — iter-52-skills-first-structural-reorder

**[!REALIZATION]** The structural inversion is now complete. The page's scroll order matches the operator-stated reader journey for the first time. The next question the loop cannot answer is the cold-reader test: does the reader feel recognition within 3 seconds of landing on the Trail or Intent card? Execute after this commit.

## 2026-05-27 — iter-52-skills-first-structural-reorder

**[!REALIZATION]** : not fired — aligns with retro-003 arc-claims

## 2026-05-27 — iter-52-skills-first-structural-reorder

**[!REVERSAL]** rather than a quiet edit.

## 2026-05-27 — iter-52-skills-first-structural-reorder

**[!REVERSAL]** "This page. Built in a single session - about 5 minutes" — the claim was true in session-001 but is no longer accurate at 52+ iterations. Removed from the Evidence item in the Improve section. The full build history is in the trail; the page doesn't need to misrepresent it.

## 2026-05-27 — iter-54-hero-skills-first-copy

**[!REALIZATION]** The iter-52 structural reorder was correctly executed but left two copy fragments pointing back to the old frame. This is the expected failure mode after large structural changes: the structure updates, the copy lags. The lag was caught in one subsequent iteration (this run), which is within normal improvement cadence.

## 2026-05-27 — iter-54-hero-skills-first-copy

**[!REALIZATION]** : not fired

## 2026-05-28 — iter-55-footer-closing-phrase

**[!REALIZATION]** : not fired — phrase placement was explicitly named as open

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** The attribution format — "Nils Wendelboe Holmager, Principles of Earned Autonomy, 2026" with DOI link — is the correct citation shape for a living document: name, title, year. The DOI link ties it to the Zenodo record, which is the stable citable artifact. This is the first time the operator's name appears in body content (not just footer attribution), associated with a specific intellectual claim.

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** : not fired

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** The gap-void pattern was identified by running de-ai on the page — and de-ai had just been updated in this same session to include this pattern class (pattern 9 spatial-void substitutes). The skill caught its own blind spot on the first run after being updated. That is the skill working as designed.

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** The principle-to-skill mapping was always implicit in the design but was never surfaced as a label. Surfacing it converts the skills section from a tool list into an argument: "here is P1, here is the skill that enacts it." That is the connection the operator was asking for. The two-tier structure is the same argument extended: "you need tier-1 immediately; tier-2 follows when you have been running long enough to need memory and arc-awareness."

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** The enumeration ("which model, which task, which day") was the de-ai tell — it is the kind of list a model generates to show it considered multiple angles. The actual claim doesn't need the examples; the reader fills them in.

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** The label was probably added early in the arc when the prose wasn't strong enough to open cold. The prose is now strong enough. The label became dead scaffolding.

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REALIZATION]** iter-68 solved one problem (unnamed principles) and created another (triple repetition). The Improve loop caught it one iteration later. This is the loop working correctly.

## 2026-05-28 — iter-56-observable-autonomy-formal-definition

**[!REVERSAL]** retro-003 operational rule 9 "Trail → Intent → Improve" superseded. New order: Intent → Trail → Improve, following principle numbering P1 → P2 → P3.

## 2026-05-28 — vision-to-destination-rename

**[!REALIZATION]** :* not fired — no prior realisation in this repo argued for or against the artifact filename.

---

**53 markers — 41 realisations, 12 reversals**
