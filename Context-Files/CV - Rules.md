# CV Rules

---

## The 33 Rules

1. **Bullet Length** — Every bullet must render on exactly one line when compiled against the current `CV - Template.tex`. A character count is never proof of this — verify by compiling; this happens at the Commit & Verify stage of the Generation Protocol below. For a starting point while drafting, check `CV - Template.tex`'s font and column width, or just draft naturally — either way, compile and confirm at that stage.
2. **XYZ Method** — Structure bullets as "Accomplished [X] as measured by [Y] by doing [Z]."
3. **Action Verbs & Active Voice** — Start every bullet with a strong engineering/business verb; the subject performs the action directly. Avoid passive voice.
4. **Quantification** — Quantify wherever an honest metric exists in the knowledge base (aim 1–2 metrics per bullet, not more). Where no metric exists, lead with concrete scope, tools, or method instead. Never invent a number to satisfy this rule — a fabricated metric is a worse failure than an unquantified bullet.
5. **Tense** — Past tense for completed roles; present tense for ongoing roles.
6. **Punctuation** — Every bullet ends with a period.
7. **No Personal Pronouns** — Eliminate I, me, my, we.
8. **ATS Layout** — Single column, no graphics or images. Multi-column layout is acceptable only where the template explicitly supports it (e.g. compact Education/Languages rows) — don't flag those as violations. Use conventional section headings only (Experience, Skills, Education, Projects, Certifications, Leadership) — an ATS parser is trained to recognize these labels, not a persona- or domain-flavored substitute, even where the substitute reads fine to a human.
9. **Bolding** — Bold job titles and one or two of the most critical keywords or metrics per bullet, not every instance. Bolding is for the human reviewer's scan path — ATS parses bold and plain text identically, and over-bolding reads as keyword-stuffing.
10. **Reverse Chronological** — Newest experience first, sorted by end date, not start date — an entry marked "Present" or "Ongoing" is the most recent regardless of when it started, and ranks above any entry with an actual end date, however recent. Where two entries are both open-ended, the one with an actual dated start (e.g. "Feb 2025 – Present") ranks above a bare "Ongoing" with no start date given, as the more specifically recent of the two.
11. **Structure (Early Career)** — Lead with the strongest asset: if internships outweigh projects, list Experience first; if coursework/projects outweigh work history, list Projects first.
12. **Structure (Experienced)** — Contact → Experience → Skills → Projects → Education.
13. **Operational Accuracy** — Verbs must match the level of involvement the knowledge base actually confirms — never upgrade "observed" to "implemented," "supported" to "led," etc. The knowledge base is the only authority on depth of involvement; if it's ambiguous, ask rather than assume the stronger claim.
14. **Page Length (Early Career)** — Strict 1 page.
15. **Page Length (Senior)** — Max 2 pages.
16. **Tailoring** — Mirror the job description's keywords exactly where honestly applicable.
17. **Coursework** — Convert coursework into "Projects" with specific deliverables.
18. **GPA** — Include only if it reflects above-average standing on the *institution's actual scale*, as documented in the knowledge base — never assume a standard 4.0-scale where higher is better. Follow the employer's posting if it explicitly requests a GPA, regardless of standing.
19. **Contact Info** — Name, phone, email, LinkedIn/GitHub (clickable).
20. **Word Count** — 450–650 words per page, optimal.
21. **Scope-Based Density** — Bullet count scales with a role's recency and relevance: 2–3 for older or less-relevant roles, 3–5 for most roles, up to 5–6 for the current or most relevant one. Expand toward the upper end only where the entry demonstrates proficiency across multiple distinct hard-skill domains.
22. **No Buzzwords** — Delete clichés like "hard worker" or "team player."
23. **No AI Clichés** — Delete "spearheaded," "leveraged," "navigated," "tapestry," and similar.
24. **Template Structure** — Follow `CV - Template.tex`'s command set (see its command reference block). Never invent new formatting commands.
25. **Hyperlinks** — Use `\href` for links.
26. **Symbol Usage** — Standard LaTeX symbols for ranges and comparisons.
27. **Spacing** — Governed by the template's spacing commands; don't hand-tune vertical spacing per entry.
28. **List Config** — Minimal indentation to maximize text width; use the template's list commands, not raw `itemize`.
29. **Acronyms** — Define on first use, then abbreviate.
30. **Date Format** — "Mon YYYY – Mon YYYY" or "Present."
31. **Math Consistency** — Numbers must align logically across bullets (e.g. a stated sample size matches a stated pass rate).
32. **The "So What?" Test** — Every bullet must state impact, not just task. If a bullet only describes what was done with no consequence, it fails this rule regardless of how well-quantified it is.
33. **Page Derivation (1-PAGE TIER)** — Every entry in `CV - Template.tex` carries a comment tag: `CORE` (always keep, as written), `TRIM` (keep the entry, but only the bullets the tag specifies — drop the rest), or `CUT` (omit the entire entry). A section built from a compact list rather than discrete entries (e.g. Skills, Languages) carries one tag for the whole section instead of per-row: `CORE` keeps every row, `TRIM` keeps only the rows the tag specifies, `CUT` omits the section — never tag a section `TRIM` if every row survives unchanged, that's `CORE`. The header carries no tag; it's always kept. To derive a 1-page version: copy the master file, apply the CUT/TRIM tags, delete the tags themselves from the result, then compile to confirm it lands on exactly one page — the tags are a guide, not a guarantee, especially after any entry changes elsewhere. This is how Rule 14's strict 1-page requirement gets executed, and it's what the Commit & Verify stage below checks alongside Rule 1.

**On duplication:** one fact lives in exactly one entry. If a fact could plausibly belong under two headings, pick the higher-impact placement and reference it briefly elsewhere if needed — never restate the same claim as if it were two separate pieces of evidence.

---

## Generation Protocol

External, one-shot document — full cost of a wrong first pass. Stop-and-wait, one stage at a time, confirm at each:

1. **Strategy** — which knowledge-base material applies, which rules are active. State it, wait for confirmation.
2. **Draft** — the full assembled bullet content, in readable form, with every rule above already applied. Wait for confirmation.
3. **Commit & Verify** — assemble the approved content into the current `CV - Template.tex`, compile, and confirm every bullet renders on one line (Rule 1) and the page count matches the intended tier (Rule 33). Fix anything that doesn't fit and recompile before delivering. Deliver the final LaTeX output.

Revisions requested *after* Commit use a lightweight changelog (original segment → new segment → reason/rule) rather than restaging from Strategy, unless the revision is substantial enough to change which knowledge-base material applies.

Subject to the fact-discipline rule in the project instructions: nothing stated beyond what the knowledge base confirms.
