# Alpha Vantage (alpha-vantage)

Alpha Vantage provides a single REST market-data API at https://www.alphavantage.co/query exposing 100+ functions across stocks (intraday/daily/weekly/monthly time series, global quote), fundamentals (income statement, balance sheet, cash flow, earnings), forex, crypto, commodities, economic indicators, technical indicators (50+ TA functions), Alpha Intelligence (news, sentiment, insider transactions, top gainers/losers), and options data. Authentication is by apikey query parameter; output is JSON or CSV.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/apis.yml)

## Tags

- Fintech
- Market Data
- Stocks
- FX
- Crypto
- Commodities
- Economic Indicators
- Technical Indicators
- Fundamentals
- News
- Sentiment
- Free

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-19

## APIs

### Alpha Vantage Market Data API

Single function-style REST endpoint that exposes the full Alpha Vantage catalog. Each call includes a function= query parameter (e.g. TIME_SERIES_INTRADAY, GLOBAL_QUOTE, OVERVIEW, INCOME_STATEMENT, RSI, FX_DAILY, CRYPTO_INTRADAY, NEWS_SENTIMENT, REAL_GDP). 20+ years of historical data, free demo key plus paid premium tiers up to 1,200 requests/min.

- **Human URL:** [https://www.alphavantage.co/documentation/](https://www.alphavantage.co/documentation/)
- **Base URL:** `https://www.alphavantage.co/query`

#### Tags

- Stocks
- Time Series
- Fundamentals
- FX
- Crypto
- Commodities
- Technical Indicators
- Economic Indicators
- News
- Sentiment
- Options

#### Properties

- [Documentation](https://www.alphavantage.co/documentation/)
- [Pricing](https://www.alphavantage.co/premium/)
- [OpenAPI](openapi/alpha-vantage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/alpha-vantage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/alpha-vantage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/alpha-vantage-inc)
- [Portal](https://www.alphavantage.co/)
- [Documentation](https://www.alphavantage.co/documentation/)
- [Pricing](https://www.alphavantage.co/premium/)
- [Git Hub](https://github.com/RomelTorres/alpha_vantage)
- [Plans](plans/alpha-vantage-plans-pricing.yml)
- [Rate Limits](rate-limits/alpha-vantage-rate-limits.yml)
- [Fin Ops](finops/alpha-vantage-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
