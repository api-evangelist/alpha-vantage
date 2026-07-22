---
name: Get a stock quote and price history
description: Fetch a real-time-ish global quote and daily price history for an equity from Alpha Vantage, handling the soft rate-limit envelope correctly.
api: openapi/alpha-vantage-stock-time-series-api-openapi.yml
operations: [queryTimeSeries]
generated: '2026-07-22'
method: generated
---

# Get a stock quote and price history

All Alpha Vantage data flows through one operation — `queryTimeSeries` (`GET https://www.alphavantage.co/query`) — routed by the `function` query parameter. An `apikey` query parameter is required on every call (the key `demo` works only for documented example symbols like IBM).

## Steps

1. Resolve the ticker if unsure: call `queryTimeSeries` with `function=SYMBOL_SEARCH&keywords=<company name>` and pick the best match from `bestMatches`.
2. Get the latest quote: `function=GLOBAL_QUOTE&symbol=<ticker>`. The price is in `Global Quote."05. price"`.
3. Get history: `function=TIME_SERIES_DAILY&symbol=<ticker>&outputsize=compact` (100 most recent points) or `outputsize=full` for 20+ years. For intraday, use `function=TIME_SERIES_INTRADAY&interval=5min`.
4. Prefer `datatype=json` (or `csv` for bulk processing).

## Rules

- Errors and throttles arrive as **HTTP 200** — always check the body for `Error Message`, `Note`, or `Information` before parsing data (see `errors/alpha-vantage-problem-types.yml`).
- Free keys allow 25 requests/day and 5/minute; on a `Note` body, back off with jitter — never tight-loop retry (see `rate-limits/alpha-vantage-rate-limits.yml`).
- The surface is read-only GET; there is no idempotency-key or pagination contract (see `conventions/alpha-vantage-conventions.yml`).
