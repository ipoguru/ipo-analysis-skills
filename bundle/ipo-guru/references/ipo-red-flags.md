# IPO red-flag check (IPO Guru only)

You run a fixed checklist against IPO Guru's pages and report what triggered and why. The flag
level comes from the stated rule below, not from your judgement.

Follow the house rules in `SKILL.md`.

Page URLs and what each page holds: see `references/page-map.md`.

## Pages to read

`/search?q=` → `/ipo/{slug}`, `/ipo-review/{slug}`, `/ipo-gmp/{slug}`, `/ipo-subscription/{slug}`,
`/ipo/{slug}/promoter-details`. Then the RHP (or DRHP) from the detail page's link or the user's attachment,
for checks 7–11, 13 and 15 (sections listed in `references/page-map.md`). If you can't open it, mark those
checks "— Not checked (RHP not read)".

## The checklist

A check whose data isn't on IPO Guru is "— Not checked". It is never "clear".

| # | Check | Flag when | Weight | Where to look |
|---|---|---|---|---|
| 1 | High valuation | Post-issue P/E > peer median by 25%+; or P/E > 50x if no peers are shown | Normal | Detail › Valuation & key ratios |
| 2 | Falling revenue growth | Latest full-year income growth below the previous year's, or income fell | Normal | Detail › Three years of numbers |
| 3 | Falling EBITDA margin | Latest full-year EBITDA margin down 2+ percentage points | Normal | same |
| 4 | Weak profitability | Loss in the latest year, PAT margin < 3%, or RoNW < 10% | Normal | same + ratios |
| 5 | High debt | Borrowing / Net worth > 1.5 (skip for banks/NBFCs and say why) | Normal | same |
| 6 | Weak demand | Mainboard: final QIB < 5x or retail < 2x. SME: final total < 20x or retail < 10x. While bidding is live: "in progress" + live figure | Normal | Subscription page |
| 7 | Aggressive pricing | OFS > 70% of the issue, or pre-IPO allotments/transfers in the last year at < 50% of the issue price | Normal | Detail › Issue summary; RHP › Capital Structure |
| 8 | Promoter/legal issues | Criminal or regulatory proceedings against the company, promoters or directors | **Critical** | RHP › Outstanding Litigation; Promoter page |
| 9 | Related-party transactions | RPTs > 10% of revenue or of expenses | Normal | RHP › Related Party Transactions |
| 10 | Customer concentration | Top customer/sector > 25% or top 10 > 60% of revenue | Normal | RHP › Risk Factors; Detail › Risks |
| 11 | Supplier concentration | Top supplier > 30% or top 10 > 70% of purchases | Normal | RHP › Risk Factors |
| 12 | Weak industry outlook | Only if IPO Guru or the RHP states a slowdown/decline | Normal | Detail, review, RHP › Industry Overview |
| 13 | Recent regulatory issues | SEBI/RBI/other regulator action, penalties or show-cause notices | **Critical** | RHP › Outstanding Litigation |
| 14 | Unusual GMP movement | GMP moved > 50% of its own level within 2 days, or swung from positive to zero/negative | Normal | GMP page › trend |
| 15 | Other concerns | Negative operating cash flow in 2 of the last 3 years, auditor qualification, contingent liabilities > 25% of net worth | **Critical** if an audit qualification; else Normal | RHP › Restated Financial Information |
| 16 | Weak analyst consensus | Sentiment score < 40/100, or more analysts advise avoid than subscribe | Normal | Review page |

## Flag level (rule-based)

- **High:** any Critical flag, or 5+ Normal flags.
- **Medium:** 2–4 Normal flags.
- **Low:** 0–1 Normal flags.
- 6 or more items "Not checked" → "Flag level: incomplete — too much data missing on IPO Guru".

Print the rule next to the level, e.g. "Flag level: Medium (3 of 11 checked items flagged; rule: 2–4 = Medium)".

## Output format

1. One line: IPO name, type, status, as-of time of the live data.
2. Checklist table: # · Check · Result (🚩 Flagged / ✓ Not flagged / — Not checked) · Actual value · Threshold.
3. "Flagged items explained": 1–2 lines each, with numbers and the page section.
4. **Flag level** with its rule.
5. **What analysts say** (review page, attributed, exactly as summarised there):
   sentiment score and consensus · Listing gains · Short-term · Long-term. If there are no reviews: "awaited".
   This is in place of your own "listing gain only / medium-term / avoid" call. Never give one.
6. "What this check doesn't cover": anything not on IPO Guru or in the RHP (market conditions, news).
7. Links + disclaimer.
