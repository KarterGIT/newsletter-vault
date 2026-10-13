# AI Newsletter Vault

This is a ChatGPT-run Obsidian/GitHub newsletter workflow.

## Project weeks
- **Week 1**: October 5–11, 2026.
- **Week 2**: October 12–18, 2026.
- New weeks increment from that start date, not the ISO calendar week number.

## Visible Obsidian layout
The root `Newsletter Template.md` is the central graph node. It links to the `Week N/Week N.md` overview for every project week. Every overview links to its daily source pulls and the single full newsletter draft. Internal source links in the newsletter provide the audit trail; the original external publication URLs remain available.

```text
Newsletter Template.md
  Week 1/Week 1.md
    Sources/2026-10-07-wed.md
    Newsletter Draft.md (not created for incomplete Week 1)
  Week 2/Week 2.md
    Sources/2026-10-13-tue.md (manual test)
    Sources/YYYY-MM-DD-day.md (Wednesday, once verified)
    Sources/YYYY-MM-DD-day.md (Friday, once verified)
    Newsletter Draft.md (Sunday, once written)
```

Weekly folders contain the real files, not placeholder nodes. Obsidian Graph View hides `_system/`, `Archive/`, the README, orphaned nodes and unresolved links. Archives and internal templates remain available in the file browser.

## Schedule (Eastern)
- Monday, Wednesday and Friday, **5 PM**: collect source research and save one dated Markdown pull if verified articles were found.
- Sunday, **5 PM**: read that week's research and write one complete original `Week N/Newsletter Draft.md`. Keep status `draft` and `reviewed_by` blank until human approval.

A manual test can count as that week's source pull if the scheduled run for its slot failed. Do not create a duplicate file for the same collection.

## Research quality
Use original publications, credible established outlets, full dated articles, and original research. Verify actual claims and URLs. Exclude Reddit, unverified rumors and AI-generated news content farms. Attribute developer claims rather than presenting them as independent findings. Prefer fewer high-quality stories to padded reports.

## Important safeguards
Never create empty news notes filled with "Nothing notable this pull." If no reliable items can be verified, report the failed run without adding a node. Never create an empty draft to fill a graph slot. Do not overwrite research notes, editorial checkboxes, existing drafts or external publication history. Keep old supplementary tests in `Archive/`, hidden from the main graph.

GitHub permissions and the web connection are required for unattended writes. Report failures explicitly rather than claiming a commit that was not verified.

The older `2026-W41`/`2026-W42` folder names were ISO calendar labels, not the newsletter issue numbers; they have been replaced by actual project Week 1/Week 2 folders.
