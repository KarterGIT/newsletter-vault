# ChatGPT weekly newsletter: project-week workflow

Repository: KarterGIT/newsletter-vault, branch main.
Cadence: Sundays at 5 PM Eastern.
Project Week 1 began Monday 2026-10-05; Week 2 is October 12–18. Increment week numbers by seven-day project weeks, NOT ISO W41/W42.

1. Read `Newsletter Template.md`, `_system/sources.md`, this instruction note, `Week N/Week N.md`, all verified research in `Week N/Sources/`, and prior newsletter draft(s) for deduplication.
2. Select the most important and credible stories from the actual collected notes, honoring `[x] keep` requests where they pass verification. Follow full source URLs to confirm date, names, figures and original claims; independently cross-check high-impact disputed items when feasible. Do not recycle unverifiable old stories or add filler to meet a target.
3. Produce **one complete original newsletter** per finished week, following the root `Newsletter Template.md` section structure: introduction, headlines, relevant technical/jobs/social/world/regulatory sections, and for each feature **What this means** in clear nontechnical language. Keep original publication URLs. Add a supporting internal Obsidian link to the specific `Week N/Sources/daily note` for traceability. No cross-links to system templates.
4. Write to `Week N/Newsletter Draft.md` ONLY if a complete meaningful newsletter is ready. YAML includes `type: newsletter-issue`, `project_week: N`, `status: draft`, and blank `reviewed_by:`. It may link back to `[[Week N/Week N|Week N overview]]`. Do not publish/send the draft or create empty placeholder drafts. Do not overwrite if a draft already exists; instead report it for editor review.
5. After confirming the GitHub commit/read-back, update the weekly overview's `<!-- WEEK FILES START -->` to `<!-- WEEK FILES END -->` segment to include a single link `[[Week N/Newsletter Draft|Full newsletter draft]]` alongside its actual sources. No separate global newsletter home, no old `issues/` subfolder.
6. Preserve editorial notes, original research and archive history; provide clear factual/source exceptions and actual paths. If approvals are blocked, return full draft text and say that GitHub did not get updated.

The central visible node is `Newsletter Template.md`. It connects to each Week N hub. Each Week N hub connects to the actual three research pulls (when available) and one complete newsletter draft, giving an easy-to-follow Obsidian graph.
