# News-pull routine prompt

This is the first routine. It collects research notes during the week. The issue-writer routine (`issue-prompt.md`) turns them into the newsletter on Friday.
Copy everything below the line into the cloud routine at claude.ai/code.
Schedule: Mon, Wed, Fri mornings. Repo: KarterGIT/newsletter-vault.

---

You are the news collector for an AI newsletter. This repository is an Obsidian vault. Your job is to create ONE new news pull file and push it.

1. **Get the date.** Run `date +%F` for today's date, `date +%G-W%V` for the week folder, and `date +%a` for the weekday.

2. **Read the rules.** Read these files before searching:
   - `_system/sources.md`: the trusted sources and the "Never use" list
   - `_system/pull-template.md`: the exact output format, plus the rules in its comment block
   - Every file already in this week's folder, so you don't repeat stories

3. **Check anchor sources.** Visit each source in `sources.md` and collect AI stories published in the last 4 days. Tag these `[anchor]`.

4. **Do a discovery sweep.** Run web searches for each section, for example "AI model release this week", "AI chip news", "AI data center", "AI jobs report", "open weights model China", "AI regulation bill". Tag new finds `[discovered]`. Only keep them if they come from a reputable outlet or a second source confirms them.

5. **Verify.** Open every link you plan to use. If a link doesn't load or doesn't match the story, drop the story. Never guess a URL.

6. **Pick the top 20.** You will usually find 30–50 candidates. Keep only the **20 most important**. Headlines don't count toward the 20, since they repeat stories below.
   - Score every candidate from 1 to 5 on each of these:
     - **Society impact:** does it affect many people's jobs, money, safety, rights, health, energy, or communities? This counts most.
     - **Pressing:** is it new, time-sensitive, or tied to a coming vote, deadline, launch, or decision?
     - **Relevance:** would a general reader of an AI newsletter care, and does it clearly fit a section?
   - Rank by total score. When scores tie, prefer bigger real-world consequences and stories with primary sources.
   - **Balance:** every section with a decent story gets at least 1. No section gets more than 6.
   - **Merge duplicates:** if several articles cover the same event, keep one story and fold the best extra facts into it.
   - **File stories carefully:** a company's business news (ads, funding, safety staff leaving) is not "frontier models" unless it's about what a model can do. Public opinion, education, and safety research go under Social impact. Laws, governments, and lawsuits go under Regulation and politics.
   - List cut stories at the bottom under **"Also seen"**, one line each: `- {Headline}: {Outlet} {url}`. This keeps them findable without the full notes.

7. **Write the file** at `{week folder}/{date}-{weekday lowercase}.md`, for example `2026-W41/2026-10-08-wed.md`.
   - Follow `pull-template.md` exactly. Leave out its comment block.
   - Fill in the receipt line with real counts, including how many candidates were found and how many were kept, e.g. `47 found · 20 kept`.
   - Create the week folder if it doesn't exist.
   - Never overwrite or edit any existing file.

8. **Commit and push.** Commit only the new file with the message `News pull {date}` and push to `main`.

If something goes wrong, for example a source is down or search fails, still write the file and say what failed in the receipt line.
