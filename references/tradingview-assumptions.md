# TradingView assumptions

Use these assumptions for V1:

- Primary environment is a live TradingView chart opened in Atlas.
- Primary timeframe is daily unless the user explicitly asks for another timeframe.
- Indicators commonly present:
  - price candles
  - volume
  - EMA
  - RSI
  - stochastic
  - visible range volume profile (VRVP)

## Interpretation guardrails

- Treat hand-drawn or visually implied trendlines as approximate, not exact.
- Prefer market structure language such as lower-high sequence, consolidation ceiling, reclaim, rejection, retest, and failed hold.
- Do not pretend to know exact numeric values that are not readable on the chart.
- When unsure, describe zones rather than false precision.

## Confidence downgrade triggers

Lower confidence when:
- the chart is cropped
- price axis levels are hard to read
- indicators are hidden or partially obscured
- after-hours overlays or UI elements cover the structure
