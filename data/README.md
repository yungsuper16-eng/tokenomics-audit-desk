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
  basis, and a stated basis for the figures. Anything that cannot be
  verified to that standard is left out. The calendar is a watch list, not a scrape.

## Fields

| Field | Meaning |
|---|---|
| `token` | Token symbol |
| `project` | Project name |
| `date` | Unlock date (UTC) |
| `amount_tokens` | Tokens released at this event |
| `pct_of_supply` | The release as a percentage of supply |
| `pct_basis` | What that percentage is **of** — total supply or circulating supply, exactly as published |
| `type` | `cliff`, `linear`, or `final` — stated only where a verified figure documents it |
| `status` | `scheduled`, or `contested — pending primary-source re-verification` |
| `source_note` | The basis for the figures; any disagreement between published figures is stated here |

## Contested figures

Where published figures disagree on a date or a size, the entry is
flagged `contested` — figures are never silently resolved. A contested
entry is verified against the project's own disclosures before any
Unlock Watch edition relies on it.

## Update cadence

The calendar is refreshed with each Unlock Watch edition, and every
figure in an edition is re-verified the morning that edition publishes.

## Sources

Entries are sourced from the projects' own published audits and
disclosures, and from published unlock schedules. Every figure is
independently verifiable.

## License

MIT — see the repository [LICENSE](../LICENSE). Use the data freely,
including commercially, with attribution.

## Citation

Analysts citing this dataset, please use:

> Tokenomics Audit Desk (2026). *90-Day Unlock Calendar* [Data set].
> GitHub. https://github.com/yungsuper16-eng/tokenomics-audit-desk/blob/main/data/unlock-calendar-90d.csv
