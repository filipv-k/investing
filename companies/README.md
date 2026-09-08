# Companies — long-term monitoring

One file per tracked company: `companies/{TICKER}.md`. Each file has four parts so the full history of a name lives in one place, available to every future conversation:

- **Profile** — snapshot facts, stance, position. Edited in place.
- **Thesis** — the full argument for why you watch/buy/sell, broken into testable *pillars*, a valuation view, and pre-committed *kill criteria*. Edited in place; versioned when the argument itself changes.
- **Validation Log** — append-only. Tracks whether the thesis is playing out, scoring each pillar confirming/neutral/contradicting over time. Deeper, lower cadence.
- **Analysis Log** — append-only. Routine price/metric/news refresh. Shallower, higher cadence.

## How the loop works
1. **Deep-dive** — first-time analysis. Creates `{TICKER}.md` from `_TEMPLATE.md`, fills Profile + Thesis (pillars, valuation, kill criteria), and writes the first Validation + Analysis entries.
2. **Monitoring update** — refresh an existing name. Reads the current Thesis and last entries for context, refreshes prices/metrics/news, appends an Analysis entry, and — if anything touches a pillar — a Validation entry too. Flags kill-criteria hits.
3. **Thesis review** — deliberate re-check of the argument: re-score pillars, revise or version the thesis, log it in the Validation Log.
4. **Portfolio review** — runs the monitoring update across every file and summarizes what changed and which theses are weakening.

## Conventions
- Filenames use the ticker in caps: `ASML.md`, `MSFT.md`.
- Dates are `YYYY-MM-DD`.
- Newest log entry goes directly under the `## Analysis Log` heading.
- `_TEMPLATE.md` is the blank starting point — copy it, don't edit it.

## Currently tracked
<!-- Keep this list updated as names are added. -->
- GOOGL — Alphabet Inc.
- GRPN — Groupon, Inc.
- NAVN — Navan, Inc.
- NOW — ServiceNow, Inc.
- P — Everpure, Inc. (ex-Pure Storage)
- SAP — SAP SE
