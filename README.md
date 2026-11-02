# Monthly literature screening

This repository holds the group's literature screening profile, so that anyone with access can run the monthly journal review with their own Claude session.

## What's here

| File | Purpose |
|---|---|
| `selection-rules.md` | The screening profile: journals to monitor (Tier A/B), 14 topic clusters with keywords, include/exclude rules, 0–6 scoring, tags, and the ready-made task prompt (section 5). |
| `reviews/` | One file per finished monthly review, named `YYYY-MM.md`. Create the folder with the first review. |
| `CLAUDE.md` | Short pointer so a Claude session opened on this repo knows what to do. |

## Running the monthly screening

1. **Open a Claude session on this repository** (Claude Code on the web, desktop or CLI, with `wdomi/lk_literature_review` attached).
2. **Give it the month.** Paste this, replacing the month:

   > Run the monthly literature screening for **October 2026** following `selection-rules.md`. Use the task prompt in section 5 and the output format there. Save the result to `reviews/2026-10.md`.

3. **Inputs.** If the session has web access, Claude fetches the tables of contents of the Tier A journals itself. If it doesn't, or if a publisher blocks it, paste or upload the tables of contents (journal "current issue" pages, RSS feeds or e-mail alerts) and say which journals they cover.
4. **Check the result.** Skim the list, delete anything off-target, and look at the "Borderline" section at the end for papers worth adding back.
5. **Save and share.** Ask Claude to commit `reviews/YYYY-MM.md`, then post it to the group as usual.

Each paper comes out in this form:

```
→ <Title> by <First author> et al. (<Journal>) <DOI>
<One-sentence summary>
Topics: <T-codes and keywords>  |  Score: <n>  |  Tags: <#tag #tag>
```

Tags: `#ibex` `#amphibians` `#plants` `#methods` `#review` `#opinion` `#data` (definitions in section 4.6 of `selection-rules.md`).

## Changing the rules

Edit `selection-rules.md` directly, or ask Claude to do it ("add journal X to Tier A", "add a #fish tag"). Keep the task prompt in section 5 in sync with any format change, since that is what the monthly run follows. The names of people who posted or recommended papers are never included in the output.
