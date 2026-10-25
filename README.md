# Tokenomics Audit Desk

Tokenomics audits graded from public on-chain data — the same engine, the
same rubric, whether the verdict comes back Sound or Fragile.

Every audit grades five things:

- **Supply** — issuance, inflation, and burn mechanics
- **Unlocks** — vesting schedules and upcoming supply events
- **Holder concentration** — who actually controls the float
- **Value accrual** — whether the token captures the protocol's economics
- **Red flags** — a scored register of everything that failed the checks

These are economic triage from public data — not smart-contract security
audits, not financial advice, no price predictions.

## Published audits (free, in full)

| Protocol | Chain | Verdict | Red-flag score |
|---|---|---|---|
| [Aave (AAVE)](reports/aave.html) | ethereum | Sound | 3.5/100 — Low |
| [Aerodrome Finance (AERO)](reports/aero.html) | base | Fragile | 72.5/100 — High |
| [Jupiter (JUP)](reports/jup.html) | solana | Sound | 13.7/100 — Low |
| [Jito (JTO)](reports/jto.html) | solana | Needs work | 31/100 — Guarded |
| [LayerZero (ZRO)](reports/zro.html) | ethereum | Needs work | 44.5/100 — Elevated |
| [Lido DAO (LDO)](reports/ldo.html) | ethereum | Sound | 5.6/100 — Low |
| [Morpho (MORPHO)](reports/morpho.html) | base | Fragile | 74.5/100 — High |
| [Raydium (RAY)](reports/ray.html) | solana | Sound | 13.7/100 — Low |
| [Uniswap (UNI)](reports/uni.html) | ethereum | Sound | 7.4/100 — Low |

Live portfolio: https://tokenomics-portfolio.pages.dev

## Open data — 90-day unlock calendar

The desk's dated unlock watch list, published as open data:

- [unlock-calendar-90d.csv](data/unlock-calendar-90d.csv)
- [unlock-calendar-90d.json](data/unlock-calendar-90d.json)

**Coverage:** 2026-10-25 through 2027-01-23 (90 days). The calendar
currently carries **3 dated events** — every unlock inside that window
that the desk has verified and placed on its Unlock Watch calendar. It
is deliberately small: an entry appears only when the desk holds
verified figures for it, never scraped in bulk and never padded. The
calendar is refreshed with each Unlock Watch edition, and every figure
is re-verified the morning its edition publishes.

**Fields:** `token`, `project`, `date`, `amount_tokens`,
`pct_of_supply` (with `pct_basis` — the share is stated against total
or circulating supply, exactly as the source states it), `type`
(`cliff`, `linear`, or `final` — only where a verified source
documents it), `status`, and `source_note`.

**Contested figures:** when public trackers disagree on a date or
size, the entry is flagged `contested — pending primary-source
re-verification` and the disagreement is named in its `source_note`.
A contested entry is never presented as settled: the desk resolves it
from the project's own disclosures before the edition publishes, or
the edition holds. The Ethena (ENA) entry is currently flagged this
way.

The calendar is the data behind
[Unlock Watch](https://tokenomics-portfolio.pages.dev/unlock-watch.html),
which also publishes on Substack —
[tokenomicsauditdesk.substack.com](https://tokenomicsauditdesk.substack.com/)
(free subscriptions). Live portfolio:
https://tokenomics-portfolio.pages.dev

Full tokenomics audit — supply, unlocks, holders, value accrual,
comparative analysis, red flags. PDF report in 48 hours. **$500, paid
in USDC on Base.** Contact: audiauditdesk@gmail.com

## Get yours

Full tokenomics audit — supply, unlocks, holders, value accrual,
comparative analysis, red flags. PDF report in 48 hours. **$500, paid in USDC on Base.**

Contact: audiauditdesk@gmail.com
