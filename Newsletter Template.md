---
type: newsletter-template
---

# Newsletter Template

This is the central template for writing weekly AI newsletters. Each week has its own research notes and one finished **draft**. The files below are linked here so the Obsidian graph stays organized.

<!-- WEEKS START -->

## Weeks
- [[Week 1/Week 1|Week 1 · October 5–11, 2026]]
- [[Week 2/Week 2|Week 2 · October 12–18, 2026]]
- [[Week 3/Week 3|Week 3 · October 19–25, 2026]]
- [[Week 4/Week 4|Week 4 · October 26–November 1, 2026]]
- [[Week 5/Week 5|Week 5 · November 2–8, 2026]]
- [[Week 6/Week 6|Week 6 · November 9–15, 2026]]
<!-- WEEKS END -->

## Newsletter writing format

**Goal:** A polished, website-ready *editorial draft* for a general audience. Source-pull Markdown is internal research; it is **not** the copy to post. The Sunday newsletter should read like a finished publication, pending fact-check and human approval.

### Style and selection rules
- Aim for roughly **900–1,300 words** on a normal week, adjusting for meaningful news. A strong shorter issue beats filler.
- Lead with the week's strongest shared theme, not a chronology of Monday/Wednesday/Friday pulls. Give the reader a reason to care in the first few lines.
- Include 3–4 concise clickable headlines followed by **5–8 well-chosen original stories**. One or two lead features may be longer; make smaller updates brief.
- Use clear paragraphs, memorable specific headings, and transitions. Vary paragraph and story lengths. Explain unfamiliar jargon naturally. Avoid hype, stock phrases and the same three-sentence summary formula for every story.
- Explain the consequences for readers or businesses *within the reporting*. Don't repeat **What this means:** after every item; use a labeled takeaway only when it genuinely improves understanding.
- Keep verified names, dates and figures. Attribute unverified benchmarks, company promises, research estimates and disputed assertions. Cite the **original linked articles** naturally in each section.
- No Reddit or unsourced rumors, inflated predictions, news-copy imitation, duplicate stories or forced category filler. Omit quiet sections rather than adding "Nothing notable".
- Preserve the established broad headings below where relevant, but choose compelling *story headlines* underneath them.
- Keep the issue `status: draft` until a human signs off. Do not send or publish automatically.

## Reader-facing issue structure

```markdown
---
type: newsletter-issue
project_week: {N}
status: draft
reviewed_by:
---

# {An interesting editorial headline, not just "Week N"}
*Week {N} | {date range}*

**{One-sentence standfirst: what defined this week's AI news}**

{An opening hook and short introduction, 2-3 paragraphs connecting the biggest developments.}

## Headlines
- **[{Big news headline}]({original URL})**: {one crisp, factual sentence}
- {2-3 more genuinely important items}

## Technical
### Frontier models: {story-specific subheading}
{Engaging original reporting and the real implications. Link to the original verified publication inline.}

### Hardware: {story-specific subheading}
{Write only if there is a meaningful distinct story.}

## Jobs
### {story-specific subheading}
{What changed for workers and employers, with quantified uncertainty.}

## Broader social impact
### {story-specific subheading}
{Social, scientific, community and data-center impacts.}

## China and open weights
### {story-specific subheading}
{Relevant global development and its significance.}

## Regulation and politics
### {story-specific subheading}
{Explain precisely whether a proposal, policy, court action or opinion.}

## The takeaway
{A concrete, thoughtful 2-4 sentence close looking ahead rather than repeating the intro.}
```

Keep only sections supported by substantial verified stories. The placeholders in this template are not article content.

## Editorial and website handoff

- The **main body** of `Week N/Newsletter Draft.md` should be readable as the site newsletter with almost no rewriting, though approval is still required.
- Keep **external article links** in the reader-facing text. For source tracing, keep Obsidian note backlinks to the week and supporting daily pulls in an **editorial-only appendix or hidden Markdown comment at the bottom**, clearly separated from the public article body.
- The Week N overview supplies the visible Graph View link to the newsletter. Avoid unnecessary cross-links or operational prompt mentions in the main prose.
- Before posting to the site, remove the YAML metadata and any editorial-only appendix, confirm links display correctly in the site's publishing system, and obtain human approval. No automatic publishing.
- Final pass: check headline/standfirst, readability aloud, internal consistency, full story dates, attribution, external URLs, tone, and no unsupported certainty.
