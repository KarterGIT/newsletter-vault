# ChatGPT news-pull task: reference instructions

**Platform:** ChatGPT Scheduled Tasks, connected GitHub integration and built-in web search.
**Repository:** `KarterGIT/newsletter-vault`, default branch `main`.
**Schedule:** Monday, Wednesday and Friday at 5:00 PM Eastern.
**Manual test:** ask ChatGPT "Run the newsletter news pull now."

The task should do the following:

1. Determine the current Eastern date and ISO week (`YYYY-Www`). Read `_system/sources.md`, `_system/pull-template.md`, every pull in the current week's folder, and the most recent issue in `issues/` if present. Preserve all existing files and never repeat an already covered event as new.
2. Search the listed anchor sources plus a broad, independent discovery sweep across AI frontier models, chips, employment, research, data-center impacts, open weights and public policy. Prioritize news published **since the previous successful pull**, normally the last 3 to 4 days. For a failed prior pull, cover the gap while clearly identifying older catch-up items.
3. Use current web research to open the *actual article URL*. Confirm its publisher, publication date, and every major factual assertion. Prefer primary announcements and original studies, Reuters, and reputable established reporting. Use at least a second source for serious controversial claims when practicable. Company releases establish what companies said, **not** independent proof of performance.
4. Exclude Reddit, social-only rumors, unknown AI-generated content farms, syndicated rewrites without original sourcing, fabricated links, inaccessible claims and advertisements masquerading as reporting. Do not infer a date from a search engine snippet when the linked article disagrees. Attribute uncertain projections and unverified claims explicitly.
5. Select **up to 20** strong distinct stories total, preferably balanced across categories, but *do not fill quotas*. Score by real-world impact, importance, freshness, reader relevance and source quality. Merge repeated coverage of one event; keep at most 6 items in any one section. Use checked/unchecked `keep` boxes as in the template. Headlines are a duplicate shortlist and do not count toward 20.
6. Write one new UTF-8 Markdown **research pull** at `YYYY-Www/YYYY-MM-DD-day.md`, using `_system/pull-template.md` including YAML metadata, accurate counts, checked source facts, URLs, and all category headings. Add `## Other research this week` with working Obsidian wikilinks to `[[YYYY-Www/YYYY-Www-index|Week overview]]` and all OTHER pull files already in that week. Never link to a file that does not exist.
7. Create and commit the new pull to `KarterGIT/newsletter-vault` on `main`; verify by reading it back. Also create or update `YYYY-Www/YYYY-Www-index.md`, a weekly Obsidian overview linking to every existing research pull and any existing issue draft. Use full vault-relative wiki links such as `[[2026-W42/2026-10-13-tue|Tuesday's research]]`. If the index exists, update **only** between `<!-- AUTO-LINKS START` and `<!-- AUTO-LINKS END -->` to preserve human editor notes outside the markers. Modify the index only after the pull has been committed successfully. Do not rewrite old research pulls when new ones arrive; older files can reach new pulls through the index and Obsidian Backlinks. Report both GitHub file paths.
8. If the web source or GitHub connector requires an interactive approval, fails, or is inaccessible during an unattended run, do **not** hang or claim to have pushed. Use other credible sources, identify failures, and return a Markdown draft in the result if committing is blocked. Never promise no permission prompts; flag any blocker for user intervention.

Do not run old cloud routines or invoke another AI service to do the research.
