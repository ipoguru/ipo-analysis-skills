# IPO Analysis Skills by IPO Guru

AI skills that analyse Indian IPOs (mainboard and SME) using **only [IPO Guru](https://www.ipoguru.in) data**
and the company's own RHP/DRHP. They work in Claude, Claude Code, ChatGPT, Gemini and any assistant that
supports the Agent Skills format.

Ask things like:

- *"Analyse the Mahanadi Coalfields IPO"*
- *"Red-flag check on the latest SME IPO"*
- *"Which mainboard IPOs are open this week with GMP above 15%?"*
- *"Compare these two IPOs on fundamentals, risks and analyst views"*

Every answer gives its figures with the IPO Guru page (and RHP page number) they came from, shows the date and time
for GMP and subscription, and ends with a disclaimer.

## The skills

| Skill | What it does |
|---|---|
| [`ipo-fundamentals`](skills/ipo-fundamentals/SKILL.md) | Balanced report on one IPO: business, 3-year financials, valuation, issue structure, demand, strengths and risks, and the analyst consensus with each analyst's verdict and the listing / short-term / long-term view |
| [`ipo-deep-dive`](skills/ipo-deep-dive/SKILL.md) | Institutional-style deep dive: business model and moat, accounting red flags, fresh issue vs OFS, valuation vs peers, promoters, litigation, related-party transactions. Every claim is cited to an IPO Guru page or an RHP page number |
| [`ipo-red-flags`](skills/ipo-red-flags/SKILL.md) | 16-point risk checklist with published thresholds and a rule-based Low / Medium / High flag level |
| [`ipo-demand-screener`](skills/ipo-demand-screener/SKILL.md) | Ranks open and upcoming IPOs by a Demand Score that combines GMP %, subscription and analyst sentiment (separate bands for SME), with optional filters such as a GMP threshold |
| [`ipo-ask`](skills/ipo-ask/SKILL.md) | Answers a specific question, or compares up to 5 IPOs side by side |

## Install

### Claude Code

```
/plugin marketplace add ipoguru/ipo-analysis-skills
/plugin install ipo-analysis@ipoguru
```

### Claude (claude.ai and Claude Desktop)

1. Download the skill you want from [`dist/`](dist/) (e.g. `ipo-fundamentals.zip`).
2. In Claude, open **Settings → Capabilities**, make sure Skills are turned on, and upload the zip.
3. Keep web search turned on, because the skills read ipoguru.in pages.

### Gemini CLI

```
gemini extensions install https://github.com/ipoguru/ipo-analysis-skills
```

### ChatGPT and the Gemini app

Create a Custom GPT or a Gem by following [`custom-assistants/README.md`](custom-assistants/README.md).
It takes about five minutes.

### Other assistants with Agent Skills support

Copy the folders inside [`skills/`](skills/) into your assistant's skills directory.

## How the skills stay on IPO Guru data

- **Sources:** pages on ipoguru.in, plus the company's RHP/DRHP opened from the IPO Guru link or attached by you.
  No other websites, news sites or model memory.
- **Missing data:** anything not found is reported as "Not available on IPO Guru", never estimated.
- **Analyst opinions:** buy/avoid views shown are the analysts' own, as tracked on each IPO's
  [review page](https://www.ipoguru.in/ipo-review/mahanadi-coalfields-ipo), with the sentiment score and every
  analyst's verdict. The assistant never adds a verdict of its own.
- **GMP:** always described as unofficial grey-market data, with its timestamp.

## Useful IPO Guru pages

[Live IPO GMP](https://www.ipoguru.in/live-ipo-gmp) ·
[Live subscription](https://www.ipoguru.in/ipo-subscription) ·
[Mainboard IPOs](https://www.ipoguru.in/mainboard-ipos) ·
[SME IPOs](https://www.ipoguru.in/sme-ipos) ·
[Analyst scoreboard](https://www.ipoguru.in/analyst) ·
[IPO performance](https://www.ipoguru.in/ipo-performance) ·
[IPO data API](https://github.com/ipoguru/ipo-gmp-api)

## Disclaimer

These skills report information published by IPO Guru and in company offer documents. They are not investment
advice. Analyst views belong to the respective analysts; IPO Guru does not make buy or sell recommendations.
GMP is unofficial and is not a reliable guide to listing price. Read the RHP and consult a SEBI-registered
adviser before investing. AI assistants can make mistakes, so check important figures on
[ipoguru.in](https://www.ipoguru.in).

## License

MIT. See [LICENSE](LICENSE). The data belongs to IPO Guru. If you build on these skills, keep a visible link to
[ipoguru.in](https://www.ipoguru.in).
