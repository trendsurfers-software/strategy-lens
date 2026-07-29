# StrategyLens — What's New

The latest updates to StrategyLens, in plain language. Newest first.

## 0.10.0 · 29 July 2026

### New

- **Ask an AI about your backtests.** StrategyLens can now be driven directly by an AI assistant — Claude, or any other MCP-compatible client. Point it at a folder of MetaTrader 5 reports and ask it to rank them, pool them into a portfolio, or dig into a single strategy's trades, in plain language. Every number is computed on your own machine by the same engine that powers the web app, so the figures match what you see here. Your reports stay on your machine; only the results you ask for reach your AI. The new **AI Ready** page walks you through the one-time setup — it takes a config snippet, a folder, and a restart of your AI client.

### Fixed

- **Share previews show the right address.** When you shared a link to an analysis, the preview card that appears in chat apps and social feeds showed an old web address. It now shows the correct one.

## 0.9.1 · 16 July 2026

### New

- **Drop the same report again, get a copy.** Re-importing a report no longer stops to ask about duplicates — you get a fresh copy named "Your Report (1)", "(2)" and so on, ready to compare side by side.
- **Two ways to remove, clearly separated.** Right-clicking a Workbench strategy or portfolio now offers **Remove from Workbench** (takes it off the panel, keeps your data) and **Delete Completely** (permanently deletes it and all its data, after asking you to confirm).

### Improved

- **Menus you can read at a glance.** Right-click menus now show an icon next to every option, and destructive actions are marked in red.

## 0.9.0 · 16 July 2026

### New

- **See how your backtest was modelled.** Every strategy now shows whether it was tested on **real ticks** or on **1m OHLC** data — right next to History Quality on the Overview, and as its own "Tick modelling" line in Strategy details. Real-tick backtests replay actual recorded prices; 1m OHLC backtests simulate prices between one-minute bars — a difference that matters a lot when you judge fast-trading strategies. Works in every report language, and portfolios show it whenever all strategies used the same data.

### Fixed

- **Holding times on hedging accounts.** Reports from hedging accounts could show wildly wrong holding times — minutes or even days instead of seconds. Trades are now matched correctly, so the average, shortest and longest holding times agree with your MetaTrader report exactly.
- **Workbench buttons in place.** Clear All and Browse now sit at the right edge of the Workbench toolbar instead of floating in the middle on wide screens.

## 0.8.0 · 15 July 2026

### New

- **Holding time on the Overview.** See how long your trades stay open — the average, the shortest, and the longest — for a single strategy or for a whole portfolio. It reads from a few seconds up to several days.
- **Search your Workbench.** A new search box lets you filter your strategies or portfolios by name — a real time-saver once you've imported a lot of them.

### Improved

- **Newest first.** Your most recently added strategies and portfolios now show at the top of the Workbench, so whatever you just imported is right where you expect it.
- **One thing highlighted at a time.** The Workbench now highlights just the strategy *or* the portfolio you're currently viewing — never both at once.
- **Keeps your place.** The Workbench remembers how far you'd scrolled, so you don't have to start from the beginning each time you open it.

---

*StrategyLens is a free tool by [TrendSurfers](https://trendsurfers.io). Open it any time at [strategy-lens.app](https://strategy-lens.app).*
