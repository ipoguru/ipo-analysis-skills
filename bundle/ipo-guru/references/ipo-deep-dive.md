# IPO deep dive (IPO Guru + RHP/DRHP)

A thorough, spin-free analysis of one IPO. Every claim cites its source: an IPO Guru page section
or an RHP/DRHP page number. Verdicts and scores come only from the analysts IPO Guru tracks.

Follow the house rules in `SKILL.md`.

Page URLs and what each page holds: see `references/page-map.md`.

## Citations

- IPO Guru: `[page › section]`, e.g. `[/ipo/mahanadi-coalfields-ipo › Three years of numbers]`.
- Offer document: `(RHP p. 312)` / `(DRHP p. 88)`.
- Company claims (market leadership, market size, moat) are the company's own statements. Label them
  "Company states… (RHP p. X)".
- Where IPO Guru and the RHP differ, give both figures and their sources. Don't pick one.

## Sources to read

1. `/search?q=` → `/ipo/{slug}`, `/ipo-review/{slug}`, `/ipo/{slug}/promoter-details`,
   `/ipo-gmp/{slug}`, `/ipo-subscription/{slug}`, and the lead-manager page(s) linked from the detail page.
   Open `/analyst/{slug}` only for the analysts listed on this IPO (their track record).
2. The RHP (or the DRHP if there is no RHP yet): use the user's attachment, or the link on the IPO Guru detail page.
   Read only the sections listed under "Reading an RHP/DRHP" in `references/page-map.md`.
   If you can't open PDFs on this platform, say so, ask the user to attach it, and continue with
   IPO Guru data, marking RHP-only items "Not checked — RHP not read".

## Report format

**1. Business model and competitive position**
- Core operations: what it does, revenue streams, customers, markets.
- Industry: market size, growth drivers, competition, entry barriers, regulation, from IPO Guru or the
  RHP's Industry Overview (labelled as the company's commissioned report).
- Moat: list the company's stated strengths, and next to each, the evidence in the numbers (margins vs
  peers, RoCE, market share, retention). Don't rate the moat yourself.

**2. Financial performance and quality**

| Period | Total income | EBITDA | EBITDA % | PAT | PAT % | Net worth | Borrowing | Citation |
|---|---|---|---|---|---|---|---|---|

Ratios from "Valuation & key ratios": RoCE, RoNW, EPS, NAV. From the RHP's restated financials:
operating cash flow, total debt, debtor days and inventory days (with page numbers).
Accounting watch-list (report each with its source, or "not observed"): operating cash flow persistently
below PAT · receivables growing faster than revenue · large "other income" share of profit · changes in
accounting policy · auditor qualification or emphasis of matter · contingent liabilities vs net worth ·
rising debt · margin compression · PAT growing much faster than income.

**3. IPO structure and use of proceeds**
- Fresh issue ₹X cr (Y%) vs OFS ₹X cr (Y%), who is selling, and the sellers' average cost per share if
  the RHP discloses it. List pre-IPO allotments/transfers in the last year and their price (RHP › Capital Structure).
- "Where the money goes" table.
- Describe it factually: "Z% of the issue goes to selling shareholders; the company receives ₹A cr." No label.

**4. Valuation**
- P/E (pre/post), market cap, NAV / price-to-book from IPO Guru. EV/EBITDA and EV/Sales at the upper band,
  using EV = market cap + debt − cash, with figures and pages from the RHP.
- Peers: the RHP's "Basis for Offer Price" table (the company chose these peers; say so), set against the
  IPO's own multiples. State the position as a fact: "post-issue P/E 38x vs peer median 31x".
- Valuation verdict: give the analysts' view from the review page, attributed. Don't add your own
  undervalued/fair/expensive label.

**5. Promoters, governance and risks**
- Promoter background, holding before/after, and pledged shares (IPO Guru + RHP › Our Promoters).
- Lead managers' track record (from the detail page / lead-manager page).
- Related-party transactions: size relative to revenue/expenses, and the trend (RHP › Related Party Transactions).
- Litigation: counts and amounts by category (criminal, tax, regulatory, civil), flagging anything involving
  promoters or directors (RHP › Outstanding Litigation).
- Top 3 risks: the three most material Risk Factors, backed by numbers (customer concentration %,
  supplier concentration %, regulatory dependence), each with its page.

**6. Analyst verdict and score** (from the review page)
- Sentiment score __/100 · consensus label · X of Y recommend subscribing · how analysts voted.
- Table: Analyst · Verdict · that analyst's track record from `/analyst/{slug}` (e.g. hit rate), if shown.
- Dual horizon view, exactly as summarised on the review page:
  **Listing gains** · **Short-term strategy** · **Long-term strategy**.
- Demand context: GMP (as-of, trend), subscription by category (as-of), anchors.
- If there are no reviews yet: "Analyst verdict: awaited", and give the data sections only.

End with "Things to verify" (3 items), the links used, and the disclaimer.
