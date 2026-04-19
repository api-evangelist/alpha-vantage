# Alpha Vantage (alpha-vantage)

Alpha Vantage is a financial data platform providing real-time and historical market data for stocks, options, cryptocurrencies, forex, commodities, and economic indicators. The API supports 50+ technical indicators, fundamental data, Alpha Intelligence sentiment analysis, and earnings data, all accessed through a single query endpoint using function-based routing.

**Website:** [https://www.alphavantage.co/](https://www.alphavantage.co/)
**Documentation:** [https://www.alphavantage.co/documentation/](https://www.alphavantage.co/documentation/)
**API Key:** [https://www.alphavantage.co/support/#api-key](https://www.alphavantage.co/support/#api-key)

## APIs

### Alpha Vantage Market Data API

Real-time and historical financial data via function-based routing on a single `/query` endpoint.

- **Base URL:** `https://www.alphavantage.co`
- **OpenAPI:** [openapi/alpha-vantage-openapi.yml](openapi/alpha-vantage-openapi.yml)
- **JSON Schema:** [json-schema/alpha-vantage-global_quote-schema.json](json-schema/alpha-vantage-global_quote-schema.json)
- **JSON-LD Context:** [json-ld/alpha-vantage-context.jsonld](json-ld/alpha-vantage-context.jsonld)
- **Capability:** [capabilities/shared/market-data.yaml](capabilities/shared/market-data.yaml)

## Generated Artifacts

| Directory | Count | Description |
|-----------|-------|-------------|
| `openapi/` | 1 | OpenAPI 3.0.3 specification |
| `json-schema/` | 8 | JSON Schema (draft 2020-12) files |
| `json-structure/` | 8 | JSON Structure documentation files |
| `json-ld/` | 1 | JSON-LD 1.1 context file |
| `examples/` | 8 | Example JSON files |
| `capabilities/shared/` | 1 | Per-API Naftiko capability definition |
| `capabilities/` | 1 | Workflow capability composition |
| `rules/` | 1 | Spectral ruleset (15 rules) |
| `vocabulary/` | 1 | Domain vocabulary and taxonomy |

## Authentication

Pass your API key as the `apikey` query parameter on all requests:

```
GET https://www.alphavantage.co/query?function=GLOBAL_QUOTE&symbol=IBM&apikey=YOUR_KEY
```

Free tier: 25 requests/day. Premium plans available at [alphavantage.co/premium](https://www.alphavantage.co/premium/).

## Key Functions

| Function | Description |
|----------|-------------|
| `TIME_SERIES_DAILY` | Daily OHLCV stock prices |
| `GLOBAL_QUOTE` | Latest real-time stock quote |
| `SYMBOL_SEARCH` | Search stocks by company name |
| `OVERVIEW` | Company fundamentals and financial ratios |
| `NEWS_SENTIMENT` | News articles with AI sentiment scores |
| `RSI` | Relative Strength Index |
| `MACD` | Moving Average Convergence/Divergence |
| `CURRENCY_EXCHANGE_RATE` | Forex/crypto exchange rates |
| `REAL_GDP` | US Real GDP economic data |

## Capability Workflows

The [financial-data-analytics.yaml](capabilities/financial-data-analytics.yaml) capability supports three research workflows:

- **Equity Research** — Combine price history, fundamentals, and news sentiment
- **Technical Analysis** — RSI, MACD, and Bollinger Bands for trading signals
- **Macro Economic Research** — GDP, unemployment, and CPI monitoring

## Maintainer

Kin Lane — kin@apievangelist.com
