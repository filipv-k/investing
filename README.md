# investing

A research notebook for a concentrated, long-term equity portfolio. One Markdown file per company, each holding the full history of that name: the current thesis, the numbers it rests on, and an append-only record of whether it is playing out.

The point of the repo is **memory**. Every claim is written down with its source so that a later read — by me or by an AI assistant picking the file up cold — can tell what was believed, when, on what evidence, and what would have to happen to change it.

## Layout

```
companies/           one file per tracked name: {TICKER}.md — the directory IS the roster
  _TEMPLATE.md       blank starting point — copy it, don't edit it
  {TICKER}_resources/  raw source material kept verbatim (transcripts, legal analyses, saved articles)
research/            dated macro / thematic notes: "YYYY-MM Topic.md"
resources/           reference reading (books, long-form PDFs) — background, not current data
.agents/skills/      agent skills for the workflows below (not populated yet)
```

Stance, conviction and position for each name live in that file's Profile — the only place they are written down.

## The per-company file

Four parts, and the split between them is the whole design:

| Part | Mode | Purpose |
| --- | --- | --- |
| **Profile** + **Watch metrics** + **Upcoming events** | edited in place | snapshot facts, stance, conviction, position, the numbers to refresh, the calendar |
| **Thesis** | edited in place, versioned | the argument: one-liner, full case, testable **pillars**, a valuation view, pre-committed **kill criteria** |
| **Validation Log** | append-only, newest first | is the *thesis* working? each pillar scored confirming ✅ / neutral ➖ / contradicting ❌. Lower cadence, deeper |
| **Analysis Log** | append-only, newest first | routine refresh: price, metrics, news. Higher cadence, shallower |

Deep-dived files add three more sections below the logs:

- **Appendix — Numbers** (`A1`, `A2`, …) — quarterly trend tables, guidance history, balance sheet, segment detail. Figures live here so the thesis prose stays short and the next update has something to diff against.
- **Appendix — Legal & regulatory** — live cases, each with a **thesis link** line saying whether and how it actually touches a pillar, plus a materiality verdict.
- **Sources** — every filing, transcript, release and data page used, linked. Non-negotiable.

Never rewrite a log entry to match a later view. The record of having been wrong is the most useful thing in the file.

## Workflows

1. **Deep-dive** — first analysis of a name. Copy `_TEMPLATE.md` → `{TICKER}.md`, fill Profile and Thesis (pillars, valuation, kill criteria), build the number appendices from primary filings, write the first Validation + Analysis entries.
2. **Monitoring update** — read the current Thesis and the last entries first, then refresh prices/metrics/news and append an Analysis entry — plus a Validation entry if anything moved a pillar. Flag any kill criterion that has been hit.
3. **Thesis review** — deliberate re-check of the argument. Re-score every pillar, revise or version the thesis, record the change and the reason in the Validation Log.
4. **Portfolio review** — run the monitoring update across all files, then summarize what changed and which theses are weakening.

## Conventions

- **Tickers in caps** for filenames: `GOOGL.md`, `SAP.md`. Dates are `YYYY-MM-DD`, always absolute — never "last quarter" or "recently".
- **Newest log entry goes directly under its `##` heading**, in both logs.
- **Numbers come from primary sources**: SEC filings and exhibits, company earnings releases and transcripts, official statistics. ČNB rates for FX. Secondary coverage is allowed for colour and market reaction, and is labelled as secondary in `## Sources`.
- **Every figure is traceable.** If a number has no source it does not go in the file.
- **State the currency.** Mixed reporting and trading currencies are normal here (SAP reports in EUR, trades in both).
- **Pillars must be falsifiable** — each carries *Confirms if* / *Breaks if* / *Current status*. A pillar you cannot break is an opinion, not a pillar.
- **Kill criteria are written before they are needed**, and quoted verbatim when triggered.
- **Theses are versioned** (`v1 → v2`) when the argument changes shape, not when a number is refreshed.
- **Quality bar:** `companies/GOOGL.md` and `companies/NAVN.md` are the reference standard for depth and sourcing.

## Open gaps

- `companies/_TEMPLATE.md` lags the live files — no Upcoming events, number appendix, legal appendix or Sources section.
- `NOW.md` is still template-shaped; `SAP.md` has the thesis (v2, short case) but not the appendix treatment.
- `.agents/skills/` is empty — the four workflows above are the obvious candidates.
- `research/` holds one note, from September 2026, and macro notes go stale fast.

---

*Personal research notes. Not investment advice. Figures are point-in-time as sourced and go stale quickly.*
