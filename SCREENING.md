# How to run the monthly literature screen

This is a quick guide for anyone in the group who needs to run the monthly journal screen with their own Claude session. All the rules Claude needs are in [`selection-rules.md`](selection-rules.md); this page tells you how to set the session up and what to paste.

## 1. Where to run it (important)

A full screen pulls the tables of contents of all Tier A journals from **Crossref** (`api.crossref.org`), with **OpenAlex** (`api.openalex.org`), **Europe PMC** (`www.ebi.ac.uk`) and **PubMed** (`eutils.ncbi.nlm.nih.gov`) for abstracts and for the author and species searches.

**Claude's default cloud sessions (claude.ai/code, Claude projects) cannot reach these APIs**: the network policy blocks them. A screen run there falls back to web searches and misses many papers. Use one of these instead:

- **Recommended: Claude Code on your own computer**, on the university network or VPN. Clone this repo, open Claude Code in the folder and paste the prompt below. (This is how the June to November 2026 screen was done.)
- **Cloud session with the domains allowed**: create a custom environment whose network access allows `api.crossref.org`, `api.openalex.org`, `www.ebi.ac.uk` and `eutils.ncbi.nlm.nih.gov`, then attach this repo.
- **Remote Control**: from a cloud session, start a Remote Control session on a computer that is on the university network.

OpenAlex has a daily quota shared by everyone behind the same university IP, so it can run out. Crossref and Europe PMC are enough on their own; tell Claude to skip OpenAlex if it starts returning errors.

## 2. What to give Claude

- This repository (in particular `selection-rules.md`).
- The date range, for example `2026-11-01 to 2026-11-30`. Papers count by **online publication date**, not issue date.
- Nothing else is needed. If a journal or database is unreachable, you can paste or upload tables of contents (journal "current issue" pages, RSS or e-mail alerts) and say which journals they cover.

## 3. Ready-to-paste prompt

Replace the dates and paste this into the session:

```text
Run the monthly literature screen for papers published online from 2026-11-01 to 2026-11-30,
following selection-rules.md in this repo (section 4.0 priority picks first, then sections 4.1–4.5,
output format in section 5).

Method:
1. For each Tier A journal, pull every record in the date range from the Crossref API
   (filter by ISSN and from-online-pub-date / until-online-pub-date; use from-pub-date only
   when no online date is registered). Add Tier B journals and bioRxiv only where relevant.
2. Priority picks: search Crossref, Europe PMC and PubMed (and OpenAlex if it works) across ALL
   journals and preprints for the group authors (Lukas Keller / Keller LF, Iris Biebach,
   Alice Brambilla) and the focal species (ibex incl. Capra spp., song sparrow, bearded vulture,
   Cinclus cinclus). Confirm author identity by affiliation when the name is ambiguous.
3. Rank the remaining records by the topic keywords in section 3, screen titles, then read
   abstracts (Europe PMC / PubMed / Crossref) for the top candidates and score them per 4.4.
4. Keep every priority pick, plus at most the 20 best other papers. Put score-2 and near-miss
   papers in a short Borderline list.
5. Check that every DOI resolves.

Output, in the section 5 format (short entries: title; journal · first author et al.; DOI;
one distilled sentence; Topics by name | Score | Tags):
- "## Important" (priority picks), then the top 20, then "Borderline".
- Start with two lines on method and gaps (journals with no abstracts, sources that failed).
- Save as reviews/YYYY-MM.md plus a plain-text copy reviews/YYYY-MM.txt for copy-pasting.
```

If you are not working inside a clone of the repo, also upload `selection-rules.md` to the session.

## 4. Check and share the result

1. Skim the Important list. Check any author match flagged as uncertain (e.g. a different "Keller").
2. Look at Borderline for papers worth moving up.
3. Read the "gaps" line: if a database failed, the screen may be incomplete for those journals.
4. Ask Claude to commit the files in `reviews/`, then send the `.txt` version to the group.

## 5. Changing the rules

Edit `selection-rules.md` directly, or ask Claude ("add journal X to Tier A", "add species Y to the priority picks"). Keep section 5 in sync with any format change, since that is what each run follows.
