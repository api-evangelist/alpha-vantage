---
name: Run technical analysis on a ticker
description: Compute moving averages, RSI, MACD, and Bollinger Bands for an equity using Alpha Vantage's technical indicator functions.
api: openapi/alpha-vantage-stock-time-series-api-openapi.yml
operations: [queryTimeSeries]
generated: '2026-07-22'
method: generated
---

# Run technical analysis on a ticker

Technical indicators are functions on the single operation `queryTimeSeries` (`GET /query`). Every indicator call needs `symbol`, `interval` (`1min`-`60min`, `daily`, `weekly`, `monthly`), and usually `time_period` and `series_type` (`close`, `open`, `high`, `low`).

## Steps

1. Trend: `function=SMA&symbol=<ticker>&interval=daily&time_period=50&series_type=close` (and `time_period=200` for the long average); `function=EMA` for exponential.
2. Momentum: `function=RSI&interval=daily&time_period=14&series_type=close` — values above 70 suggest overbought, below 30 oversold.
3. Convergence: `function=MACD&interval=daily&series_type=close` — compare `MACD` vs `MACD_Signal` crossovers.
4. Volatility: `function=BBANDS&interval=daily&time_period=20&series_type=close` for upper/middle/lower bands.
5. Corroborate with raw prices from `function=TIME_SERIES_DAILY` before drawing conclusions.

## Rules

- One indicator = one request. The free tier is 5 requests/minute and 25/day — plan the indicator set before calling, and back off on a `Note` body (HTTP 200 soft throttle; see `rate-limits/alpha-vantage-rate-limits.yml`).
- Always check for `Error Message`/`Note`/`Information` fields in the 200 body before parsing (see `errors/alpha-vantage-problem-types.yml`).
- The MCP server (`https://mcp.alphavantage.co/mcp`) exposes each indicator as a same-named tool with a typed inputSchema — prefer it in agentic contexts (see `mcp/alpha-vantage-tool-crosswalk.yml`).
