# History

Auto-generated from `.trail/audit-trail.md` by the `record.py history --write` command in the autonomous-agent-skills install.
Do not edit by hand — re-run the command to refresh.

| # | Date | Slug | Outcome | Delta |
|---|------|------|---------|-------|
| ▸ 1 | 2026-05-26 | session-001 — repo-init + vision |  |  |
| ▸ 2 | 2026-05-26 | session-002 — improve-iter-1 — build index.html |  |  |
| ▸ 3 | 2026-05-26 | session-003 — improve-iter-2 — sharpen time claim |  |  |
| ▸ 4 | 2026-05-26 | session-004 — improve-iter-3 — intellectual lineage |  |  |
| ▸ 5 | 2026-05-26 | session-005 — improve-iter-4 — Monokai dark colour scheme |  |  |
| ▸ 6 | 2026-05-27 | session-006 — improve-iter-5 — credible external links |  |  |
| ▸ 7 | 2026-05-26 | session-008 — improve-iter-7 — light theme |  |  |
| ▸ 8 | 2026-05-26 | session-007 — improve-iter-6 — CSS architecture + illustrations |  |  |
| ▸ 9 | 2026-05-27 | iter-26 - trail-section-rebuild |  |  |
| ▸ 10 | 2026-05-01 | iter-35-prose-simplification |  |  |
| ▸ 11 | 2026-05-27 | iter-36-dark-theme-section-scoped-accents |  |  |
| ▸ 12 | 2026-05-27 | iter-37-footer-de-ai-followup |  |  |
| ▸ 13 | 2026-05-27 | iter-38-semantic-colour-system |  |  |
| ▸ 14 | 2026-05-27 | iter-39-vision-run-design-direction |  |  |
| ▸ 15 | 2026-05-27 | retro-002-arc-read |  |  |
| ▸ 16 | 2026-05-27 | iter-40-hero-copy-recognition |  |  |
| ▸ 17 | 2026-05-27 | iter-41-de-ai-pass |  |  |
| ▸ 18 | 2026-05-27 | iter-43-cold-audit-p3-tagline |  |  |
| ▸ 19 | 2026-05-27 | iter-44-hero-secondary-cta |  |  |
| ▸ 20 | 2026-05-27 | iter-44-hero-secondary-cta |  |  |
| ▸ 21 | 2026-05-27 | iter-45-get-started-nav |  |  |
| ▸ 22 | 2026-05-27 | iter-46-nav-order-get-started-before-trail |  |  |
| ▸ 23 | 2026-05-27 | iter-47-inline-style-cleanup |  |  |
| ▸ 24 | 2026-05-27 | iter-48-github-pages-push |  |  |
| ▸ 25 | 2026-05-27 | iter-49-repo-rename |  |  |
| ▸ 26 | 2026-05-27 | iter-50-title-deai-pass |  |  |
| ▸ 27 | 2026-05-27 | retro-003-skills-first-reorientation |  |  |
| ▸ 28 | 2026-05-27 | iter-52-skills-first-structural-reorder |  |  |
| ▸ 29 | 2026-05-27 | iter-53-quickstart-copy-and-reference |  |  |
| ▸ 30 | 2026-05-27 | iter-54-hero-skills-first-copy |  |  |
| ▸ 31 | 2026-05-28 | iter-55-footer-closing-phrase |  |  |
| ▸ 32 | 2026-05-28 | iter-56-observable-autonomy-formal-definition |  |  |
| ▸ 33 | 2026-05-28 | vision-to-destination-rename | artifact `.trail/vision.md` renamed to `.trail/destination.md` to match the renamed Destination skill (was Vision; now at `destination/SKILL.md` v2.0.0 in the skills suite, commit e3d1577). H1 header updated to match; no other content in destination.md was modified — it remains operator-held. | artifact filename only; skill behaviour unchanged. |

### Run 8 — 2026-05-26 — session-007 — improve-iter-6 — CSS architecture + illustrations

- **decided:** One change: hero copy rewrite
- **decided:** Shorten P2/P3 taglines + promote tagline visual weight
- **decided:** Two factual fixes in one iteration
- **decided:** One comprehensive copy clarity pass
- **decided:** marker, truncation note, and link to full trail on GitHub. Added "Trail" nav anchor. Added ~70 lines of CSS using existing :root tokens.
- **decided:** Footer statement � full-width row below name/links, above license
- **REVERSAL:** trail entry.** Session-1 Vision required self-referential proof. Iter-8 removed it. No individual trail entry marks this as a reversal. The Vision run (session-9) caught it retrospectively.
- **REVERSAL:** on retro-001 arc-claim #4
- **REVERSAL:** marker and corrected text. Claim #6 updated to remove browser check as an open item. Browser check removed from "What the next runs should test" and operational rules.
- **REVERSAL:** Vision constraint overridden by operator
- **REVERSAL:** : a Vision-level constraint was removed by operator direction, not by agent initiative.
- **REVERSAL:** iter-17 author voice draft was wrong

### Run 9 — 2026-05-27 — iter-26 - trail-section-rebuild

- **decided:** Replace the single wrong-source entry with a .trail-scroll container holding the three curated skills-suite entries. Keep 'View full trail on GitHub' link outside the scroll wrapper so it stays anchored regardless of scroll position. Rewrite the section intro to make the source explicit ('the skills suite's own audit trail - the loop running on itself').
- **decided:** Add a new section id="memory" between the existing skills section and the trail section. Content: section label "Memory Model", title "The .trail/ folder is the memory", a monospace directory tree using box-drawing characters with each filename highlighted, a definition-list-style grid explaining each file's role using a "where you're going / where you are / what you've learned / the path you walked" framing, and a closing paragraph on the disagreement-resolution hierarchy.
- **decided:** Replace the four-item structure with the complete seven-item structure. Update the directory tree to use box-drawing for the two subdirectories with one example filename each. Add three new memory-file rows (history.md, sessions/, transcripts/). Add a three-tier paragraph above the per-file grid (operator / synthesis / evidence) so the reader sees the grouping that makes seven items legible instead of overwhelming.
- **decided:** Insert a new section id="quickstart" between Memory Model and Trail. Four-card grid (one per step), each card containing: step number + time, title, one-sentence body, monospace code block(s), and a "done when" gate. Closing paragraph with optional commit-hook step and a link to the full QUICKSTART.md on GitHub.
- **decided:** Three steps, each one line of code, presented as a numbered ol with large accent-coloured counter numbers in the left gutter. One short intro: "Step 1 runs in your terminal. Steps 2 and 3 are chat commands to the agent." - this is the one piece of context that the bare commands cannot communicate (which interface receives them). One closing line that names what success looks like, plus a single link to the full QUICKSTART.md for anyone who wants the long version.
- **decided:** Incremental change. iter-33 = typography + weight + tracking + radius. iter-34 (deferred, candidate next move #1) = spacing.
- **decided:** Kaikaku â€” full v2 in one iter.**
- **REVERSAL:** Within-iteration scope broadening: `git add -A` swept a pre-existing deletion of `content/image.png` into the iter-33 commit. The file was orphaned (no grep hits anywhere in the repo) so the deletion is correct, but it was not in my stated scope. Lesson: when working in a repo with possible operator-side pending changes, use `git add <specific-files>` not `-A`. Recording this rather than silently passing it off.
- **REVERSAL:** ` lesson). Commit `fc45ea3`: 424 insertions, 931 deletions.

### Run 11 — 2026-05-27 — iter-36-dark-theme-section-scoped-accents

- **decided:** One incremental change with a structural twist
- **REVERSAL:** Vision-contradicting move

### Run 12 — 2026-05-27 — iter-37-footer-de-ai-followup

- **decided:** Two-artifact iteration.

### Run 13 — 2026-05-27 — iter-38-semantic-colour-system

- **decided:** Replace section-scoped accent with semantic type-driven colour roles

### Run 16 — 2026-05-27 — iter-40-hero-copy-recognition

- **decided:** Two text changes: h1 and subhead; meta description updated to match

### Run 18 — 2026-05-27 — iter-43-cold-audit-p3-tagline

- **decided:** Rewrite P3 tagline

### Run 19 — 2026-05-27 — iter-44-hero-secondary-cta

- **decided:** Wrap hero button in `.row`, add `.chip.chip-lg` link to `#principles`

### Run 20 — 2026-05-27 — iter-44-hero-secondary-cta

- **decided:** Wrap hero button in .row, add .chip.chip-lg link to #principles

### Run 21 — 2026-05-27 — iter-45-get-started-nav

- **decided:** Add 'Get started' nav item before GitHub ↗

### Run 22 — 2026-05-27 — iter-46-nav-order-get-started-before-trail

- **decided:** Swap Trail and Get started in nav

### Run 23 — 2026-05-27 — iter-47-inline-style-cleanup

- **decided:** Add utility classes, replace all 24 violations

### Run 26 — 2026-05-27 — iter-50-title-deai-pass

- **decided:** Three changes:

### Run 28 — 2026-05-27 — iter-52-skills-first-structural-reorder

- **decided:** Execute the full structural reorder as one atomic iteration. All four sub-changes are interdependent: reordering sections without updating nav creates broken navigation; expanding Improve without moving it above Principles still buries the key skill. Split execution would leave the page in an intermediate broken state.
- **REVERSAL:** rather than a quiet edit.
- **REVERSAL:** "This page. Built in a single session - about 5 minutes" — the claim was true in session-001 but is no longer accurate at 52+ iterations. Removed from the Evidence item in the Improve section. The full build history is in the trail; the page doesn't need to misrepresent it.

### Run 29 — 2026-05-27 — iter-53-quickstart-copy-and-reference

- **decided:** Replace "Three commands" (bash install.sh / /vision / /improve) with: one-sentence copy instruction + 6-row reference table using existing memory-row CSS. No new CSS. Skill order matches the skills section above (Trail → Intent → Improve → Vision → Retrospect → Probe). Each row: when to invoke (bold) + produces (inline).

### Run 30 — 2026-05-27 — iter-54-hero-skills-first-copy

- **decided:** Two string replacements: hero paragraph + meta description. Both "Three principles" → "Six skills." Meta description updated to: "...Six skills that close that gap — for any model, any toolset." No structural or CSS changes.

### Run 31 — 2026-05-28 — iter-55-footer-closing-phrase

- **decided:** Add <p class="mono small center mt-md">Delegate to AI. Own the work.</p> between the footer paragraph and the license line. No new CSS classes — mono, small, center, mt-md all pre-exist.

### Run 32 — 2026-05-28 — iter-56-observable-autonomy-formal-definition

- **decided:** Add the quote as a semantic <blockquote> with <cite> and DOI attribution in the Observable Autonomy section, immediately after the informal tagline "Autonomy is earned through transparency." Add lockquote CSS using existing design tokens (lavender border, ink text, muted attribution). No new tokens needed.
- **decided:** Apply all four gap-void-substitute removals as a single iter-57 change. Same root pattern, same session that identified it, no structural risk.
- **decided:** Kaikaku on the skills section. Six changes in one iteration:
- **decided:** Compress second response to two sentences. Move the punch line ("wrong after it had already been used") to the end position. Cut the enumeration ("which model, which task, which day").
- **decided:** Remove all three instances. Same class, same pattern, same fix. One iter.
- **decided:** Two cuts: P2 third parallel sentence removed; ARF callout second clause folded into the first.
- **decided:** Strip announcement frame, fix word repetition: "I had this problem: how to delegate real work to AI and stay accountable for it."
- **decided:** Move Foundations to last section before footer. Update nav to match: Skills → Principles → Get started → Trail → Foundations.
- **decided:** Remove the card entirely. H1 → CTA → Skills. No intermediate problem-framing detour.
- **decided:** Remove both. Hero is now label + h1 only. The skills section opens immediately below.
- **decided:** --gap-lg: 3rem → 2rem. Single token, uniform effect.
- **decided:** The heading is the name of the framework. "Three Principles" described the count; "Principles of Earned Autonomy" names the thing. The eyebrow label "Why the skills work" is retained for context.
- **decided:** Remove the hero label. H1 stands alone: "You're delegating real work to AI. Stay accountable for the work." No eyebrow needed — the statement is self-contained.
- **decided:** Operator supplied the anchor: "Force the AI to understand the intent behind the prompt." Previous versions (iter-70, iter-71) were too complex. Final: "Forces the AI to understand the intent behind your prompt, not just the words. The principle behind military command, Socratic method, and coaching kata."
- **decided:** Operator: "use the orange color for headers instead of purple." --amber (#e7c97a) is the amber/orange token. .label was on --lavender. Single token swap in .label rule. :root comment updated to reflect new semantic roles: amber=labels/headers, lavender=conceptual emphasis (em, blockquote borders — unchanged).
- **decided:** Replace .stack-lg + 3 .principle divs with .grid-3 + 3 .card divs. Each card: label (P[n] · Name), mono tagline, 2-sentence description, link to PRINCIPLES.md.
- **decided:** Updated all 9 occurrences in one pass: skill card (h3 link text + URL /vision/SKILL.md → /destination/SKILL.md + produces reference), Improve loop step 1 (read destination.md), memory tree filename, memory tier description, memory-row key, hierarchy note (vision wins → destination wins), quickstart skill name + produces reference.
- **REVERSAL:** retro-003 operational rule 9 "Trail → Intent → Improve" superseded. New order: Intent → Trail → Improve, following principle numbering P1 → P2 → P3.

### Run 33 — 2026-05-28 — vision-to-destination-rename

- **decided:** Run the mechanical migration in pea-website: `git mv .trail/vision.md .trail/destination.md`, update the H1 header line only, leave the rest of the file untouched (operator-held content per the vision-management discipline), append this entry, regenerate derived artifacts, commit only the migration-related files, push.

**33 runs total — 33 with changes, 0 silence**
