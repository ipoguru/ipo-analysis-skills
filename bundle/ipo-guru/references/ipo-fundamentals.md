# IPO fundamentals (IPO Guru only)

You build a balanced report on one IPO from IPO Guru's pages. The opinions in it are the
analysts' opinions as IPO Guru tracks them, never yours.

Follow the house rules in `SKILL.md`.

Page URLs and what each page holds: see `references/page-map.md`.

## Pages to read

1. Find the IPO: `/search?q=<name>`. If several match, ask the user which one. If none match, say
   IPO Guru doesn't cover it and stop.
2. Read: `/ipo/{slug}` (detail) and `/ipo-review/{slug}` (review). Also read `/ipo-gmp/{slug}` if
   GMP is quoted and `/ipo-subscription/{slug}` if bidding has started.

## Report format

Use these headings in this order. Keep each section short, and use tables for numbers.

**1. Snapshot** — name, mainboard/SME, exchanges, timetable (open / close / allotment / listing),
price band, lot size, minimum investment, issue size, status.

**2. Analyst view at a glance** (from the review page)
- Sentiment score __/100 · consensus label · "X of Y analysts recommend subscribing"
- Table: Analyst · Verdict (exactly as listed)
- If there are no reviews yet: "Analyst consensus: awaited". Don't add a substitute view.

**3. Company and products** — what it does, how it earns money, products/services, customers,
markets (from "About the company"). One short paragraph.

**4. Industry and sector** — only what IPO Guru's pages say. If there are no industry figures, say so.

**5. Financial trend** (from "Three years of numbers")

| Period | Total income | YoY growth | EBITDA | EBITDA margin | PAT | PAT margin | Net worth | Borrowing |
|---|---|---|---|---|---|---|---|---|

Show the formula for YoY growth and margins the first time. Label part-year periods (e.g. 6 months to Sep)
and don't compare them with full years. Add 3–5 bullets on direction: growth speeding up or slowing,
margins widening or shrinking, PAT growth vs revenue growth, debt trend. Cash flow: "Not available on IPO Guru" unless the
page shows it.

**6. Valuation** (from "Valuation & key ratios") — P/E pre and post issue, EPS, market cap,
RoCE, RoNW, margins, NAV. Peers: only if IPO Guru lists them, otherwise "Peer comparison not available
on IPO Guru". State figures as facts. Don't call the valuation cheap or expensive.

**7. Issue structure** — fresh issue vs OFS (₹ cr and %), who is selling, "Where the money goes",
promoter holding before → after, lead managers and their track record (from the detail page).

**8. Demand signals** — GMP (₹, %, as-of time, trend direction from the GMP page); subscription by
category with as-of time; anchor allocation if done; allotment probability if shown.

**9. Strengths and risks** — from the detail page's "Strengths & risks" (company-stated; say so).
Add a weakness only where the numbers above show one directly (e.g. "PAT fell from ₹11,842 cr to ₹10,698 cr").

**10. What the analysts say, by horizon** (from the review page's Detailed review)
- **Listing gains:** the analysts' view, as summarised by IPO Guru
- **Short-term:** …
- **Long-term:** …
Quote or closely paraphrase. Don't add anything of your own. If a part is missing, write "No analyst view yet".

**11. Before you decide** — 3 specific things to check (e.g. final QIB subscription on closing day, the
allotment date, the RHP's risk factors), the links used, and the disclaimer.
