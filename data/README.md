# 90-Day Unlock Calendar — dataset notes

The Tokenomics Audit Desk's dated unlock watch list, published as open
data. This is the dataset behind
[Unlock Watch](https://tokenomics-portfolio.pages.dev/unlock-watch.html).

## Files

- `unlock-calendar-90d.csv` — one row per dated unlock event
- `unlock-calendar-90d.json` — the same events, structured, with
  coverage metadata

## Coverage

- **Window:** 2026-10-25 through 2027-01-23 (90 days) at this revision
- **Events:** 13 dated events at this revision
- **Inclusion rule:** an entry appears only when the desk holds verified
  figures for it — token, date, amount, the share of supply with its
  basis, and a named source. Anything that cannot be verified to that
  standard is left out. The calendar is a watch list, not a scrape.

## Fields

| Field | Meaning |
|---|---|
| `token` | Token symbol |
| `project` | Project name |
| `date` | Unlock date (UTC) |
| `amount_tokens` | Tokens released at this event |
| `pct_of_supply` | The release as a percentage of supply |
| `pct_basis` | What that percentage is **of** — total supply or circulating supply, exactly as the source states it |
| `type` | `cliff`, `linear`, or `final` — stated only where a verified source documents it |
| `status` | `scheduled`, or `contested — pending primary-source re-verification` |
| `source_note` | Where the figures come from; any disagreement between trackers is named here |

## Contested figures

When public trackers disagree on a date or a size, the entry is flagged
`contested` and the disagreement is named in its `source_note` — figures
are never silently resolved. A contested entry is resolved from the
project's own vesting and unlock disclosures before any Unlock Watch
edition relies on it, or the edition holds.

## Update cadence

The calendar is refreshed with each Unlock Watch edition, and every
figure in an edition is re-verified the morning that edition publishes.

## Sources

Entries are sourced from the projects' own published audits and
disclosures held by the desk, and from public unlock trackers —
principally DefiLlama's unlocks pages and Tokenomist — cross-checked
against each other. Each entry's `source_note` names its own sources.

## License

MIT — see the repository [LICENSE](../LICENSE). Use the data freely,
including commercially, with attribution.

## Citation

Analysts citing this dataset, please use:

> Tokenomics Audit Desk (2026). *90-Day Unlock Calendar* [Data set].
> GitHub. https://github.com/yungsuper16-eng/tokenomics-audit-desk/blob/main/data/unlock-calendar-90d.csv
