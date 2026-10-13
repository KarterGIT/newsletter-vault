# ChatGPT weekly issue-writer task: reference instructions

**Platform:** ChatGPT Scheduled Tasks with GitHub read/write.
**Repository:** `KarterGIT/newsletter-vault`, default branch `main`.
**Schedule:** Sunday at 5:00 PM Eastern.
**Manual test:** ask ChatGPT "Test the newsletter writer now."

1. Determine the ISO week and read `_system/newsletter-template.md`, all weekly pull files from `YYYY-Www/`, any uncovered stories from the previous week, and the most recent issue under `issues/`.
2. Treat any `- [x] keep` checkbox as an editor's selection, provided the story can still be verified. Select other important stories based on impact, reader relevance and quality; remove duplicates. Do not invent stories or pad sections.
3. Reopen the original source URL for every featured item. Verify names, figures, dates and substantive claims; distinguish claims from evidence. If a source no longer works, obtain a reliable independent source or omit the claim.
4. Draft an **original, accessible** newsletter following `_system/newsletter-template.md`. Explain what happened and `**What this means:**` for nontechnical readers. Explain jargon in context. Attribute analytical uncertainty, avoid copying prose, and include a direct external article link to every featured story PLUS an Obsidian internal link to the exact dated pull note supplying it, such as `[[2026-W42/2026-10-13-tue|Research notes]]`. Do not confuse the article URL with the local Obsidian source-note link.
5. Use YAML `status: draft` and blank `reviewed_by:`; **do not publish/send** the newsletter. Keep the human review checklist from the template, including checking links and facts. If a section lacks significant verified developments, omit that section.
6. Add a `## Research notes for this issue` section listing `[[YYYY-Www/YYYY-Www-index|Week overview]]` and every dated pull from which selected stories were used, including a previous week if needed. Link only existing files. Find next issue number and commit a new `issues/YYYY-MM-DD-issue-N.md`, never overwriting an issue. Verify by fetching the new issue. Then update this week's `YYYY-Www/YYYY-Www-index.md` to link to the committed newsletter, editing **only** its marked AUTO-LINKS section. Research files can find the issue through Obsidian's Backlinks and the weekly index. Keep wiki links for internal Obsidian drafts; convert/remove them before distributing a public newsletter.
7. Report issue file path, featured story count, any source/repository failures, and which items warrant editorial review. If GitHub authorization or writing fails, return the full Markdown issue in the task result and transparently report that no commit occurred.

This is a ChatGPT workflow. It requires the connected GitHub authorization to remain valid; no unattended write can be guaranteed if permissions change.
