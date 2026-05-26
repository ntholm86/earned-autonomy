# retrospect.md — pea-website

_Last updated: 2026-05-26 (run: retro-001)_

---

## Current claims

**1. The loop has been optimizing the frame, not the painting.**
6 of 9 logged sessions targeted color, CSS, layout, links, or spacing. The primary constraint — per the Vision run — is copy and visual hierarchy for instant non-technical comprehension. The loop has been systematically finding lower-leverage changes while the highest-leverage problem (copy) sits untouched.

**2. The hero copy is 9 sessions old and was written before the audience was fully understood.**
Session-2 wrote the hero and explicitly predicted "will need at least one copy-refinement pass." That prediction is now 9 sessions old. The session-1 Vision dialogue established the audience as "both equally." Session-9 confirmed the primary reader is now the non-technical reader arriving cold. The copy was not written with that constraint in mind. It is stale by construction, not by neglect.

**3. A vision-level reversal (proof section removal) occurred without a `[!REVERSAL]` trail entry.**
Session-1 Vision explicitly required self-referential proof as a core structural element. Iter-8 removed it because it was false and audience-wrong. This is the most significant single change in the arc — a core vision constraint overturned — and it has no `[!REVERSAL]` marker in any individual trail entry. It was caught only because the Vision skill was run. Future arc-reads should treat structural section removal as a `[!REVERSAL]`-class event.

**4. ~~The browser visual check was never done.~~ — [!REVERSAL] retro-001 was wrong.**
The operator has been doing the browser visual check informally throughout the arc — it just was never trailed. It was the implicit feedback mechanism driving the majority of visual iterations: session-8 (light theme), iter-10 (density), iter-11 (typography), and all operator-initiated copy requests originated from the operator seeing the page in a browser. The check was continuous and unlogged, not deferred. The trail treated absence of a trail entry as absence of the activity — a known failure mode.

**5. The Monokai reversal (sessions 5→8) was the only major resolved reversal, and it was resolved cleanly.**
The CSS architecture investment in session-7 (semantic `:root` variables, zero inline styles) made a full palette reversal a 2-edit operation. This is the clearest concrete payoff in the arc: an architectural investment made a likely reversal cheap. The architecture is now settled and does not need revisiting.

**6. One item has been open for 7+ sessions without resolution: Chen et al. 2025.**
Appears as a "Candidate next move" in every session from session-3 onward. Not blocking publication. Should be resolved or explicitly closed — a paper citation with no link is either permanently unlinked or has a findable arXiv ID. The browser visual check is removed from this list — see claim #4.

---

## What the next runs should test

**Primary (blocking publication):**
1. **Hero restructure** — does the first screen achieve 3-second clarity for a non-technical reader? Specifically: can a reader who sees only the h1, subtitle, and any bold/visual anchors — without reading body copy — understand what PEA is and what problem it solves? If not, the hero needs to lead with the answer, not the problem setup.
2. **Principles scan test** — can a reader understand the three principles in 30 seconds by scanning structure (headings, icons, bold text) without reading body copy? If not, the visual hierarchy is doing too little work.

**Secondary (deferred, not blocking):**
3. **Chen et al. 2025** — either find and add the arXiv ID, or explicitly mark the citation as permanently unlinked text. 7 sessions of "open" with no action taken means it should be closed one way or the other.

---

## Active operational rules

- **Never add inline `style=""` attributes.** They accumulate silently across sessions and require a dedicated clean-up iteration. If a CSS class doesn't exist for the property, create one.
- **All CSS changes go through `:root` tokens.** Proven by the Monokai→light reversal: full palette swap in 2 edits. The system works. Keep it.
- **The trail's "Candidate next moves" section has low predictive validity for what actually happens next.** The operator-gate consistently redirects. Record candidate moves but treat them as weak signal — not as a commitment.
- **In this shell environment: use `Select-String` not `grep`; use `Add-Content` not `>>` for append operations on trail files.**
- **Section removal is a `[!REVERSAL]`-class event when the removed section was a vision requirement.** Mark it explicitly.
- **The hero copy has not been examined since session-2.** Any future session that touches presentation without examining copy is misallocating attention.

---

## Loop-effectiveness notes

The loop has been finding genuine work, but work of the wrong kind for this stage. The visual and architectural improvements (sessions 4–11) are real and compounding: the CSS is clean, the architecture is solid, the intellectual lineage is present. These were necessary. But they were not sufficient, and the loop consistently found another visual lever to pull rather than examining copy.

The structural bias is explicable: visual changes are concrete, testable, and reversible. Copy changes require judgment about what a non-technical reader understands — they are harder to evaluate without user feedback. The loop defaults to visual work partly because it can verify visual work. It cannot easily verify whether copy achieves instant clarity without testing against an actual cold reader.

The Vision run functioned as the corrective: it forced an arc-level look that the individual Improve iterations had been deferring. The run's primary output — "the text is not good enough, I don't get instant clarity" — names a failure that had been present in the target for 9 sessions.

**The loop is not broken. It is biased toward safe, verifiable work at the expense of high-leverage, harder-to-verify work.** The next run should be guided by the question: "What would a cold non-technical reader experience in the first 5 seconds?" — not by any CSS property or link.
