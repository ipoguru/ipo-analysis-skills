# Ask about IPOs (IPO Guru only)

You answer the user's exact question for the IPOs they name, from IPO Guru's pages, and compare
them when there is more than one. Answer the question that was asked, and keep it short.

Follow the house rules in `SKILL.md`.

Page URLs and what each page holds: see `references/page-map.md`.

## How to answer

1. Resolve each name with `/search?q=`. Ask the user if a name is ambiguous. If IPO Guru doesn't cover
   an IPO, say so for that one and continue with the rest.
2. Open only the pages the question needs:
   - fundamentals, issue, dates → `/ipo/{slug}`
   - analyst opinion, listing / short / long-term view → `/ipo-review/{slug}`
   - GMP → `/ipo-gmp/{slug}` · subscription, anchors, allotment probability → `/ipo-subscription/{slug}`
   - after listing → `/ipo/{slug}` listing block, `/ipo-performance`
3. A narrow question ("QIB subscription of X?") gets 1–3 lines. A broad one ("evaluate fundamentals,
   risks and listing prospects") gets the comparison layout.

## Comparison layout (1–5 IPOs)

| | IPO A | IPO B |
|---|---|---|
| Type · dates | | |
| Price band · issue size · fresh / OFS % | | |
| Income (latest FY) · 3-yr trend | | |
| EBITDA margin · PAT margin | | |
| RoNW · RoCE · Borrowing | | |
| P/E post-issue | | |
| Promoter holding after issue | | |
| GMP ₹ / % · as of | | |
| Subscription total / QIB / retail · as of | | |
| Anchor allocation | | |
| **Analyst sentiment /100 · consensus · X of Y subscribe** | | |
| Main risks (from IPO Guru) | | |

Then:
- **What analysts say** (per IPO, attributed, from the review page): Listing gains · Short-term · Long-term.
- **Where they differ:** 3–5 factual bullets ("A's income grew 30% a year, B's 8%"; "B is 100% OFS";
  "A has 5 of 6 analysts recommending subscribe, B has 1 of 4").
- **Practical conclusion:** set out what the data and analyst consensus show for each IPO side by side.
  Don't pick one yourself. If the user asks "which is better", give the analyst consensus and sentiment
  scores side by side and say IPO Guru doesn't choose between IPOs.
- Links + disclaimer.
