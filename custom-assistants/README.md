# Use the skills in ChatGPT or the Gemini app

Neither app installs skills from GitHub, but both let you build a custom assistant from the same files.

## ChatGPT (Custom GPT)

1. Go to **chatgpt.com → Explore GPTs → Create → Configure**.
2. **Name:** `IPO Guru IPO Analyst`. **Description:** `Indian IPO analysis from IPO Guru data`.
3. **Instructions:** paste the whole of [`instructions.md`](instructions.md).
4. **Knowledge:** upload these 6 files:
   - [`skills/ipo-fundamentals/SKILL.md`](../skills/ipo-fundamentals/SKILL.md) → rename to `ipo-fundamentals.md`
   - [`skills/ipo-deep-dive/SKILL.md`](../skills/ipo-deep-dive/SKILL.md) → `ipo-deep-dive.md`
   - [`skills/ipo-red-flags/SKILL.md`](../skills/ipo-red-flags/SKILL.md) → `ipo-red-flags.md`
   - [`skills/ipo-demand-screener/SKILL.md`](../skills/ipo-demand-screener/SKILL.md) → `ipo-demand-screener.md`
   - [`skills/ipo-ask/SKILL.md`](../skills/ipo-ask/SKILL.md) → `ipo-ask.md`
   - [`skills/ipo-fundamentals/references/page-map.md`](../skills/ipo-fundamentals/references/page-map.md) → `page-map.md`
5. **Capabilities:** turn on **Web Search**. Code Interpreter is optional, and image generation can stay off.
6. **Conversation starters:** "Analyse <IPO name> IPO" · "Which IPOs are open this week?" ·
   "Red-flag check on <IPO name>" · "Compare <IPO A> and <IPO B>".

## Gemini app (Gem)

1. Go to **gemini.google.com → Gems → New Gem**.
2. Paste [`instructions.md`](instructions.md) into **Instructions**.
3. Upload the same 6 files as **Knowledge**.
4. Save. If answers ignore the page links, start each chat with "Use ipoguru.in only".
