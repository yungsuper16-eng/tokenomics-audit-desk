<p align="center"><img src="assets/logo.svg" alt="Tokenomics Audit Desk" width="120"></p>

# Tokenomics Audits & Token Unlock Calendar

**Tokenomics Audit Desk** — tokenomics audits graded from public on-chain
data, and the dated token unlock calendar the desk watches, published as
open data. The same engine, the same rubric, whether the verdict comes
back Sound or Fragile.

**Portfolio:** https://tokenomics-portfolio.pages.dev ·
**Unlock Watch:** https://tokenomics-portfolio.pages.dev/unlock-watch.html ·
**Substack:** https://tokenomicsauditdesk.substack.com/ ·
**Dev.to:** https://dev.to/tokenomicsdesk ·
**Order a full audit ($500):** https://tokenomics-portfolio.pages.dev/#order

## Sample audits — graded, published in full

Nine audits, free to read, every figure sourced:

| Protocol | Chain | Red-flag score | Verdict |
|---|---|---|---|
| [Aave (AAVE)](reports/aave.html) | ethereum | 3.5/100 — Low | Sound |
| [Lido DAO (LDO)](reports/ldo.html) | ethereum | 5.6/100 — Low | Sound |
| [Uniswap (UNI)](reports/uni.html) | ethereum | 7.4/100 — Low | Sound |
| [Jupiter (JUP)](reports/jup.html) | solana | 13.7/100 — Low | Sound |
| [Raydium (RAY)](reports/ray.html) | solana | 13.7/100 — Low | Sound |
| [Jito (JTO)](reports/jto.html) | solana | 31/100 — Guarded | Needs work |
| [LayerZero (ZRO)](reports/zro.html) | ethereum | 44.5/100 — Elevated | Needs work |
| [Aerodrome Finance (AERO)](reports/aero.html) | base | 72.5/100 — High | Fragile |
| [Morpho (MORPHO)](reports/morpho.html) | base | 74.5/100 — High | Fragile |

## What an audit grades

Every audit grades five things:

- **Supply** — issuance, inflation, and burn mechanics
- **Unlocks** — vesting schedules and upcoming supply events
- **Holder concentration** — who actually controls the float
- **Value accrual** — whether the token captures the protocol's economics
- **Red flags** — a scored register of everything that failed the checks

These are economic triage from public data — not smart-contract security
audits, not financial advice, no price predictions.

## Open data — the 90-day unlock calendar

The desk's dated unlock watch list, published as open data under the MIT
license (see [LICENSE](LICENSE) and [data/README.md](data/README.md)):

- [unlock-calendar-90d.csv](data/unlock-calendar-90d.csv)
- [unlock-calendar-90d.json](data/unlock-calendar-90d.json)

**Coverage:** 2026-10-25 through 2027-01-23 (90 days). The calendar
currently carries **8 dated events**. It is deliberately small: an entry
appears only when the desk holds verified figures for it, never scraped
in bulk and never padded. The calendar is refreshed with each Unlock
Watch edition, and every figure is re-verified the morning its edition
publishes.

**Fields:** `token`, `project`, `date`, `amount_tokens`,
`pct_of_supply` (with `pct_basis` — the share is stated against total
or circulating supply, exactly as the source states it), `type`
(`cliff`, `linear`, or `final` — only where a verified source documents
it), `status`, and `source_note`.

**Contested figures:** when public trackers disagree on a date or size,
the entry is flagged `contested — pending primary-source
re-verification` and the disagreement is named in its `source_note`. A
contested entry is never presented as settled: the desk resolves it from
the project's own disclosures before the edition publishes, or the
edition holds. Three entries are currently flagged this way —
EigenCloud (EIGEN) and Sui (SUI) on size or tranche composition, and
Arbitrum (ARB) on a one-day date difference between trackers. The
Ethena (ENA) entries were re-issued on 2026-10-25 from the Ethena
Foundation's own disclosures: the November figure previously carried
did not survive primary-source verification and was withdrawn, and the
two scheduled monthly tranches that replaced it are labelled with
their sourcing in their `source_note`s — one derived from Ethena's
published vesting terms, one secondary-corroborated.

The calendar is the data behind
[Unlock Watch](https://tokenomics-portfolio.pages.dev/unlock-watch.html),
which also publishes on Substack —
[tokenomicsauditdesk.substack.com](https://tokenomicsauditdesk.substack.com/)
(free subscriptions).

## Get yours

Full tokenomics audit — supply, unlocks, holders, value accrual,
comparative analysis, red flags. PDF report in 48 hours. **$500, paid
in USDC on Base.**

Order: https://tokenomics-portfolio.pages.dev/#order
Contact: audiauditdesk@gmail.com
