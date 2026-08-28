# Cloudflare App Cost Calculator

[![OpenRoots ORA 2.3](https://openroots.org/badge/ora.svg)](https://openroots.org/licenses/ora/2.3)

A single-file, client-side calculator that models the full monthly cost and profit of running an application entirely on Cloudflare. It covers Workers, Durable Objects, D1, R2, KV, Queues, Vectorize, email, security, residential-proxy scraping, LLM usage, and a push notification subsystem, then lays it against revenue so you can see margin in real time.

Live tool. https://mjmirza.github.io/cloudflare-cost-calculator/

## What it does

- A sticky profit and loss view with cost in red and revenue in green.
- A model picker for top OpenAI, Anthropic, Google, xAI, and DeepSeek models with live per-token pricing.
- Profiles from Solo to Extreme that move every sub value at once.
- A click-to-expand cost breakdown. Click any row to jump to the control that drives it.
- A profitability advisor that names the highest-impact fix first and applies it in one click.
- Market-grounded pricing with a buyer verdict and a recommended price.
- A scale-aware impact indicator on every input. If a field cannot move the numbers right now, it tells you why, for example within the free tier at this scale, retention is off, or LLM excluded from total.

## How to use it

1. Open the live tool above, or open index.html in any browser.
2. Pick a profile or a user count preset.
3. Tweak any value on the left. The figures and the breakdown update instantly.
4. Read the advisor for the next move toward your target margin.

Everything runs in the browser. There is no backend, no tracking, and no data leaves the page.

## Run locally

```bash
git clone https://github.com/mjmirza/cloudflare-cost-calculator.git
cd cloudflare-cost-calculator
open index.html
```

## License

MIT. See LICENSE.
