# IPO demand screener (IPO Guru only)

You rank live IPOs by the **IPO Guru Demand Score**, which combines three signals from IPO Guru:
GMP %, subscription, and analyst sentiment. The formula is fixed and is always shown, so the
ranking is a calculation on data, not your opinion.

Follow the house rules in `SKILL.md`.

Page URLs and what each page holds: see `references/page-map.md`.

## Inputs (use the defaults unless the user says otherwise)

- Segment: mainboard (default) / SME / both
- Status: open + upcoming (default) / open only / closed but not yet listed
- Filters (optional): GMP % ≥ X · total / QIB / retail subscription ≥ Y · sentiment score ≥ Z
- Specific IPO names, if given (screen only those)

## Pages to read

1. `/live-ipo-gmp`: every IPO with current GMP (₹, %) in one page.
2. `/ipo-subscription` (or `/sme-ipo-subscription`): live/final subscription for all IPOs.
3. For each IPO that passes the filters (max 10): `/ipo-review/{slug}` for the sentiment score and
   consensus, and `/ipo/{slug}` for the business line and dates.

## IPO Guru Demand Score (0–100)

Score each component with the bands for the IPO's segment, then average the available components.
SME IPOs routinely see far higher subscription and GMP, so they have their own bands.

| Component | Source | Mainboard points | SME points |
|---|---|---|---|
| GMP % | GMP page | ≤ 0% → 0 · >0–10% → 25 · >10–25% → 50 · >25–50% → 75 · > 50% → 100 | ≤ 0% → 0 · >0–20% → 25 · >20–50% → 50 · >50–90% → 75 · > 90% → 100 |
| Subscription (total, latest) | Subscription page | < 1x → 0 · 1–5x → 25 · >5–20x → 50 · >20–50x → 75 · > 50x → 100 | < 5x → 0 · 5–50x → 25 · >50–150x → 50 · >150–400x → 75 · > 400x → 100 |
| Analyst sentiment | Review page | the page's sentiment score /100, as is | same |

- **Demand Score = average of the available components.** Equal weights.
- When the screen covers both segments, score each IPO on its own segment's bands and show a Type column.
- Needs at least 2 of the 3 components. With only 1, the IPO goes to "Not ranked — not enough data".
- A missing component is **missing, not zero**: no GMP quoted yet, bidding not started, or reviews awaited.
- A GMP threshold filter excludes IPOs that have no GMP figure. They don't "pass" it.
- Ties: the higher QIB subscription ranks first, then the higher GMP %.

## Output format

**Screen used:** segment · status · filters · data as of <time from the pages>

| Rank | IPO | Type | Price band | GMP ₹ / % (pts) | Total subs (pts) | QIB | Retail | Sentiment /100 · consensus | **Demand Score** | Close | Listing |
|---|---|---|---|---|---|---|---|---|---|---|---|

Then for each ranked IPO, 3 lines:
- **Business:** one line (what it does, sector).
- **Analysts:** X of Y recommend subscribing, plus the review page's *Listing gains* view in one sentence, attributed.
- **Watch:** 1–2 material facts from its data (e.g. "100% OFS", "income fell last year").

Then:
- **Not ranked:** IPOs with too little data (name + what's missing).
- **How the Demand Score works** (always print this, with the bands for the segment(s) shown):
  "Demand Score = average of the available components: GMP points (<bands>), subscription points
  (<bands>) and the IPO Guru analyst sentiment score /100. Needs at least 2 of the 3. It summarises
  demand data and is not a prediction of listing gains."
- Links + disclaimer.
