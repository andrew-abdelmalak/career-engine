# CV Rules

---

## The 33 Rules

1. **Bullet Length** — Every bullet must render on exactly one line when compiled against the current `CV - Template.tex`. A character count is never proof of this — verify by compiling; this happens at the Commit & Verify stage of the Generation Protocol below. For a starting point while drafting, check `CV - Template.tex`'s font and column width, or just draft naturally — either way, compile and confirm at that stage.
2. **XYZ Method** — Structure bullets as "Accomplished [X] as measured by [Y] by doing [Z]."
3. **Action Verbs & Active Voice** — Start every bullet with a strong engineering/business verb; the subject performs the action directly. Avoid passive voice.
4. **Quantification** — Quantify wherever an honest metric exists in the knowledge base (aim 1–2 metrics per bullet, not more) — a real approximation or range ("~20%," "double-digit growth") counts as quantified if the knowledge base supports the direction and rough scale, even without an exact figure. Where no metric or credible approximation exists, lead with concrete scope, tools, or method instead. Never invent a number to satisfy this rule — a fabricated metric is a worse failure than an unquantified bullet.
5. **Tense** — Past tense for completed roles; present tense for ongoing roles.
6. **Punctuation** — Every bullet ends with a period.
7. **No Personal Pronouns** — Eliminate I, me, my, we.
8. **ATS Layout** — Single column, no graphics or images. Multi-column layout is acceptable only where the template explicitly supports it (e.g. compact Education/Languages rows) — don't flag those as violations. Use conventional section headings only (Experience, Skills, Education, Projects, Certifications, Leadership) — an ATS parser is trained to recognize these labels, not a persona- or domain-flavored substitute, even where the substitute reads fine to a human.
9. **Bolding** — Bold job titles and one or two of the most critical keywords or metrics per bullet, not every instance. Bolding is for the human reviewer's scan path — ATS parses bold and plain text identically, and over-bolding reads as keyword-stuffing.
10. **Reverse Chronological** — Newest experience first, sorted by end date, not start date — an entry marked "Present" or "Ongoing" is the most recent regardless of when it started, and ranks above any entry with an actual end date, however recent. Where two entries are both open-ended, the one with an actual dated start (e.g. "Feb 2025 – Present") ranks above a bare "Ongoing" with no start date given, as the more specifically recent of the two.
11. **Structure (Early Career)** — Under ~2 years of experience (students, recent grads). Contact → Education leads, then the strongest asset: Experience next if internships outweigh projects, Projects next if coursework/projects outweigh work history.
12. **Structure (Experienced)** — Contact → Experience → Skills → Projects → Education. A Professional Summary (Rule 33) inserts between Contact and Experience.
13. **Operational Accuracy** — Verbs must match the level of involvement the knowledge base actually confirms — never upgrade "observed" to "implemented," "supported" to "led," etc. The knowledge base is the only authority on depth of involvement; if it's ambiguous, ask rather than assume the stronger claim.
14. **Page Length (Early Career)** — Strict 1 page. Applies under ~2 years of experience (Rule 11's threshold).
15. **Page Length (Experienced)** — Max 2 pages. Roles older than roughly 10–15 years lose their bullets entirely — keep just the org, title, and dates — unless a specific bullet there still directly matches the target role.
16. **Tailoring** — Mirror the job description's keywords exactly where honestly applicable.
17. **Coursework** — Convert coursework into "Projects" with specific deliverables.
18. **GPA** — Include only if it reflects above-average standing on the *institution's actual scale*, as documented in the knowledge base — never assume a standard 4.0-scale where higher is better. Drop it roughly 2–3 years after graduation, or once the knowledge base shows several years of full-time experience, unless it's unusually strong or the employer's posting explicitly requests it regardless of standing.
19. **Contact Info** — Name, phone, email, LinkedIn/GitHub (clickable).
20. **Word Count** — 450–650 words per page, optimal.
21. **Scope-Based Density** — Bullet count scales with a role's recency and relevance: 2–3 for older or less-relevant roles, 3–5 for most roles, up to 5–6 for the current or most relevant one. Expand toward the upper end only where the entry demonstrates proficiency across multiple distinct hard-skill domains.
22. **No Buzzwords** — Delete clichés like "hard worker" or "team player." Don't claim a soft skill by name either (leadership, communication, teamwork) — demonstrate it through a quantified accomplishment instead; a bullet that shows leading a team outweighs a line that just says "leadership skills."
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
33. **Professional Summary (Experienced)** — For Experienced-tier CVs (Rule 12/15), open with a short summary before Experience: the target role or field, one sentence of scope or context, and 2–4 of the strongest accomplishments compressed to a phrase each. Skip it at Early Career — the space is better spent on Experience there.

**On duplication:** one fact lives in exactly one entry. If a fact could plausibly belong under two headings, pick the higher-impact placement and reference it briefly elsewhere if needed — never restate the same claim as if it were two separate pieces of evidence.

---

## Generation Protocol

External, one-shot document — full cost of a wrong first pass. Stop-and-wait, one stage at a time, confirm at each:

1. **Strategy** — which knowledge-base material applies, which rules are active. State it, wait for confirmation.
2. **Draft** — the full assembled bullet content, in readable form, with every rule above already applied. Wait for confirmation.
3. **Commit & Verify** — assemble the approved content into the current `CV - Template.tex`, compile, and confirm every bullet renders on one line (Rule 1) and the page count matches the required length (Rule 14 or 15). If it doesn't fit, decide what to cut or compress based on the knowledge base and the rules above (Rule 21's density guidance, Rule 32's impact test, and so on), then recompile before delivering. Deliver the final LaTeX output.

Revisions requested *after* Commit use a lightweight changelog (original segment → new segment → reason/rule) rather than restaging from Strategy, unless the revision is substantial enough to change which knowledge-base material applies.

Subject to the fact-discipline rule in the project instructions: nothing stated beyond what the knowledge base confirms.
