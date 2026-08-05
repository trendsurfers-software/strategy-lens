# StrategyLens — What's New

The latest updates to StrategyLens, in plain language. Newest first.

## 0.13.0 · 5 August 2026

### New

- **Test an idea without re-running a backtest.** Ask your AI assistant things like "what if I skipped Fridays?" or "what if I only kept long trades?" and StrategyLens recomputes every metric for that filtered set instantly — so you can find where a strategy is bleeding before you change a single EA input.
- **Try a different position size and see the new drawdown.** Have your assistant replay the same trades at a different risk level and read back the resized balance curve and drawdown — a way to explore sizing without running one backtest per guess.
- **See how much of a result was luck.** Your assistant can now run a robustness check that reshuffles your trades many times over and shows the range of outcomes, the median result, and the risk of ruin. Every run is repeatable, so the same question gives the same answer.
- **A clearer risk snapshot.** Analysing a single strategy now also surfaces its longest flat stretch, worst losing streak, biggest single loss, and a plain traffic-light verdict.

### Changed

- **Diversification is now measured day by day.** When you combine strategies into a portfolio, how closely they move together is now lined up on a shared calendar — by day, week, or month — instead of by trade order. It is more accurate, so some of your correlation and diversification-health numbers will shift, usually for the better.

## 0.12.1 · 5 August 2026

### Fixed

- **Shared strategy previews now show the right numbers.** The preview image that appears when you share a strategy link could show a total return that was far too high, a trade count that was off by one, and a start-and-end date squeezed into a single day. This happened for strategies loaded from an account history statement, where the opening deposit was mistakenly counted as trading profit. Previews now match your Overview exactly — the correct return, the right number of trades, and the full date range your trades cover. Links you have already shared are corrected automatically, so there is no need to share them again.

## 0.11.0 · 31 July 2026

### New

- **AI assistants see everything the Overview shows.** The AI interface can now return every metric from the Overview page — yearly stats, monthly P/L, long vs short split, holding times, profit in pips, per-strategy rankings, and account stats for live statements — using the new `sections` parameter. No extra computation; the engine already had the numbers, they just weren't accessible through the AI interface.
- **Full report identity in AI results.** AI results now include the EA name, timeframe, broker, leverage, data quality, tick model, and EA inputs for each report — the same details you see in the Overview header.

### Fixed

- **Backtest dates now match what you tested.** If your EA was inactive at the start of the testing window, StrategyLens used to show the date of the first trade as the start, making it look like part of your test period was missing. It now shows the actual period you configured in the Strategy Tester. This fix applies everywhere — Overview, shared portfolios, and the strategy library.

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
