# PlutoSwing

A swing-trade decision desk in a single `index.html` — no build, no dependencies.

## What's inside

- **Chart & Signal** — SVG candlestick chart with SMA 20/50/200, Bollinger bands, volume, RSI, and MACD panes; daily/weekly intervals; keyboard-navigable crosshair; a transparent long/short confluence score with every point itemized; and an ATR-based trade plan.
- **Screener** — the whole watchlist scored on the same confluence model, sortable by any column.
- **Top Picks** — watchlist ranked for a chosen holding period (1 week to 1 year), with each stock's own conditional forward-return history spelled out, sample sizes and overlap caveats included.
- **Trade Planner** — position sizing from the loss side: account, risk %, entry, stop → share count, R levels, breakeven win rate.
- **Backtest** — runs the exact on-chart score against history with next-open entries, ATR stops, R targets, and time stops; conservative same-bar stop-first fills.
- **Pluto** — the swing pup keeps watch in the corner. His collar turns green when the long side clears 65 on the open chart, red when the short side does; click him for a tip.

Ships with a 24-symbol default watchlist and a ~110-name company database (megacap tech, semis, software, fintech, financials, healthcare, consumer, energy, industrials, China ADRs, and sector ETFs) — and any other ticker can be added on top.

## Data

Starts in clearly-labeled **demo mode** (seeded, regime-switching random walks — stable per symbol). Add a free [Twelve Data](https://twelvedata.com/pricing) API key in Settings for live daily data; requests are cached for 10 minutes to stay inside the free tier.

## Run it

Open `index.html` in a browser, or:

```sh
npx serve .
```

**PlutoSwing is decision support, not financial advice.** Signals and backtests describe the past; they don't promise the future.
