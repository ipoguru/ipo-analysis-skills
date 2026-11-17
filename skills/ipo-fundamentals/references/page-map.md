## IPO Guru page map

Base: `https://www.ipoguru.in`. `{slug}` is usually `<company-name>-ipo`, e.g. `mahanadi-coalfields-ipo`.

### Finding an IPO
| Need | Page |
|---|---|
| Resolve a name to a slug | `/search?q=<name>` (open the IPO result; ask the user if several match) |
| All mainboard / SME IPOs | `/mainboard-ipos`, `/sme-ipos` (page 1 = current + upcoming + last 30 days) |
| Upcoming | `/upcoming-mainboard-ipo`, `/upcoming-sme-ipo` |
| Calendar | `/calendar-view` |

### One IPO (both mainboard and SME)
| Page | URL | What's on it |
|---|---|---|
| Detail | `/ipo/{slug}` | Timetable · Issue summary (price band, lot, issue size, fresh vs OFS) · What will it cost me · Strengths & risks · Three years of numbers (Assets, Total Income, PAT, EBITDA, Net Worth, Reserves, Borrowing) · Valuation & key ratios (P/E pre/post, EPS, RoCE, RoNW, PAT & EBITDA margin, NAV, market cap) · Where the money goes · About the company · Promoters (holding pre/post) · Bankers & filings · Documents · **Lead Manager Track Record** · Anchor investors (when done) · FAQ |
| Review | `/ipo-review/{slug}` | **Sentiment score /100 · consensus label · X of Y recommend subscribing · how analysts voted · Detailed review (General, Listing gains, Short-term strategy, Long-term strategy) · Analyst reviews table (analyst, verdict, report PDF)** |
| GMP | `/ipo-gmp/{slug}` | Current GMP (₹ and %), day-wise GMP trend, Kostak, Subject-to-Sauda |
| Subscription | `/ipo-subscription/{slug}` | Live bidding by category (QIB, NII, bNII, sNII, Retail, Employee, Shareholder) · Basis of allotment · Application-wise breakup · **Allotment probability** · Subscription insights · Day-wise history · Anchor investor allocation |
| Promoters | `/ipo/{slug}/promoter-details` | Promoter background. **Not every IPO has one**: a 404 means use the detail page's "Promoters" section |
| Allotment | `/ipo-allotment/{slug}` | Allotment status link. **Link only; never ask for a PAN in chat.** |
| RHP / DRHP | link in the detail page's "Documents" / "The bankers & the filings" | The company's offer document. Open **only** this link (or a user-attached copy) |

### Reading an RHP/DRHP (400+ pages; go to these sections, don't read cover to cover)
Summary of the Offer Document · Capital Structure (pre-IPO allotments and prices) · Objects of the Offer ·
Basis for Offer Price (the company's chosen peers, with P/E, EPS, RoNW) · Industry Overview · Our Business ·
Our Promoters and Promoter Group · Restated Financial Information (cash flow, debt) · Management's
Discussion and Analysis · Related Party Transactions · Outstanding Litigation and Material Developments ·
Risk Factors (customer/supplier concentration).

### Across IPOs
| Need | Page |
|---|---|
| Live GMP of all IPOs | `/live-ipo-gmp` (also "How GMP called the last N listings") |
| Live subscription, all IPOs | `/ipo-subscription`, `/sme-ipo-subscription` |
| Listing & post-listing returns | `/ipo-performance`, `/sme-ipo-performance` |
| Analyst scoreboard | `/analyst` · one analyst: `/analyst/{slug}` (calls at a glance, verdict mix, best/worst call, call history, SEBI registration) |
| How the sentiment score is built | `/how-we-rate` |
| Lead managers | `/lead-managers` · `/lead-manager/{slug}` |
| Anchor investors | `/anchor-investor-group`, `/anchor-investor-scheme` (+ `/{slug}`) |
| Shareholder quota | `/upcoming-ipo-shareholder-quota` |
| Pre-IPO / unlisted prices | `/pre-ipo-shares`, `/pre-ipo-shares/{slug}` |
| IPO news | `/news` |
