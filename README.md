# AI Newsletter Project

A prototype workflow for researching AI news, organizing sources in Markdown, and drafting a weekly newsletter with ChatGPT. The repository is private; nothing here is published to a website automatically.

## Start here: review the sample

**[Read the publication-style newsletter sample (October 5–11)](Tests/Publication-Ready%20Newsletter%20Preview%20-%20Week%201.md)**

This standalone sample shows the intended **writing and editorial direction**. It's deliberately not connected to the real weekly drafts. It is **not a published issue**.

Feedback would be especially useful on the target audience, story selection, depth, tone, overall length, and whether the newsletter feels close to ready for a website.

## How it works

1. **Research, Monday / Wednesday / Friday, 5 PM Eastern.** ChatGPT searches credible original sources, opens articles, checks dates and claims, filters duplicates, and saves verified notes. It doesn't make empty placeholder notes when research fails.
2. **Draft, Sunday, 5 PM Eastern.** ChatGPT revisits sources, selects important stories, and writes a reader-facing newsletter with a strong introduction, linked articles, natural explanation, and a closing takeaway.
3. **Human review.** The issue stays marked `draft` until someone checks accuracy, links, format and writing. No automatic publication.

The scheduled task prompts are kept short. Their detailed rules live in `_system/routine-prompt.md`, `_system/issue-prompt.md` and `_system/sources.md`; the publication style is in `Newsletter Template.md`.

## Where the files live

| File / folder | Purpose |
| --- | --- |
| [Newsletter Template.md](Newsletter%20Template.md) | Central week index and newsletter writing style |
| [Week 1](Week%201/Week%201.md) | October 5–11; initial research retained for reference |
| [Week 2](Week%202/Week%202.md) | October 12–18; current automation test week |
| `Week N/Sources/` | Up to three dated research collections per week |
| `Week N/Newsletter Draft.md` | One full Sunday draft, created only when written |
| `Tests/` | Standalone publication-style sample, separate from weekly drafts |
| `_system/` | Instructions and trusted source lists; not site content |

Project weeks are counted from **Monday, October 5, 2026**. They are *not* ISO calendar-week numbers.

## Current status

**Work in progress.** GitHub research and writing were tested interactively, but an entire Monday–Sunday sequence has **not** yet completed unattended. Week 1 contains earlier research that must be reverified before use; Week 2 contains a manual verified pull, with the first scheduled Sunday draft pending. Failures and missing research are reported, never filled with invented content.

Project navigation uses standard relative Markdown links on GitHub. Local editor settings and plugins are excluded from version control. External articles are linked for traceability; company claims and research estimates should be clearly attributed.
