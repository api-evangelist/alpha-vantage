---
name: Research company fundamentals
description: Pull a company overview and financial statements (income statement, balance sheet, cash flow, earnings) for an equity from Alpha Vantage.
api: openapi/alpha-vantage-stock-time-series-api-openapi.yml
operations: [queryTimeSeries]
generated: '2026-07-22'
method: generated
---

# Research company fundamentals

Fundamentals are served by the same single operation `queryTimeSeries` (`GET /query`), selected with the `function` parameter.

## Steps

1. Start with `function=OVERVIEW&symbol=<ticker>` for the company profile: sector, market cap, PE ratio, EPS, dividend yield, 52-week range. (On the MCP server this tool is named `COMPANY_OVERVIEW`.)
2. Pull statements as needed, one call each: `function=INCOME_STATEMENT`, `function=BALANCE_SHEET`, `function=CASH_FLOW` — each returns `annualReports` and `quarterlyReports` arrays.
3. Add `function=EARNINGS` for reported vs. estimated EPS history.
4. For market context, blend in `function=NEWS_SENTIMENT&tickers=<ticker>` (ticker-level sentiment scores per article).

## Rules

- Each statement is a separate request — a full fundamentals pass is ~5 calls, which is the free tier's entire per-minute budget (5/minute). Sequence calls and check every body for `Note`/`Information` (HTTP 200 soft throttling).
- Some datasets/entitlements are premium-only; an `Information` body means the key's plan does not cover the request — do not retry (see `errors/alpha-vantage-problem-types.yml`).
- Authenticate with the `apikey` query parameter on every call (see `authentication/alpha-vantage-authentication.yml`).
