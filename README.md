# Route Chat: wireframe

Wireframe for **Route Chat**, a chat interface for [route.fun](https://www.route.fun). You type what you want, and the agent either hands back the matching Route widget, prefilled (swap, limit, multi-swap, earn...), or a short rundown with sources. Nothing moves until the user signs.

Route Chat is already on Route's public roadmap ("Expand" phase, planned).

Light mode only. Single static file, no build step. Same visual language as [route-earn](https://github.com/todels/route-earn).

**Local:** `python3 -m http.server 5202 -d .` then open http://localhost:5202

## Sections

| # | Section | What it shows |
|---|---------|---------------|
| 00 | How it works | 4 rules + the flow: entry → ask → do / learn → review → sign → receipt |
| 01 | Start | Empty chat: one input, four starters |
| 02 | "buy me 7k of $ROUTE" | Assumption chips + the real swap card, prefilled |
| 03 | Review → sign → done | Widget states: review, wallet, pending, done, failed |
| 04 | "who's behind $ROUTE" | Research rundown: one-line answer, sourced fact rows, risk flags, actions |
| 05 | Every product | Limit, multi-swap, earn, screener, portfolio, analytics |
| 06 | Edge cases | Same ticker, no amount, no wallet, low balance, risky token, out of scope |
| 07 | Placement | Chat tab, chat as home, ⌘K from anywhere, history, mobile |
| Q | Open questions | What to ask the client before hi-fi |

## Rules the design follows

1. **Chat prepares, wallet signs.** The agent never moves funds.
2. **Widgets, not walls of text.** Actions use the existing Route cards.
3. **Show the guess.** Every assumption is a tappable chip.
4. **Every answer ends in a next step.**

Research facts in 04 are taken from docs.route.fun and route.fun/analytics (Oct 2026). Prices, balances and APYs elsewhere are sample numbers.
