# Alpha Vantage

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Alpha Vantage provides a single REST market-data API at https://www.alphavantage.co/query exposing 100+ functions across stocks (intraday/daily/weekly/monthly time series, global quote), fundamentals (income statement, balance sheet, cash flow, earnings), forex, crypto, commodities, economic indicators, technical indicators (50+ TA functions), Alpha Intelligence (news, sentiment, insider transactions, top gainers/losers), and options data. Authentication is by apikey query parameter; output is JSON or CSV.

**Areas:** Fintech · Market Data · Stocks · Foreign Exchange · Cryptocurrency · Commodities · Economic Indicators · Technical Indicators · Fundamentals · News · Sentiment · Free

## Alpha Vantage on APIs.io

Everything profiled for Alpha Vantage is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/alpha-vantage/](https://apis.io/providers/alpha-vantage/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Alpha Vantage Query API](https://apis.io/apis/alpha-vantage/alpha-vantage-query-api/) — The Query API from Alpha Vantage — 1 operation(s) for query.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [alphavantage](https://apis.io/servers/alpha-vantage/alphavantage/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Alpha Vantage Agentic Access](https://apis.io/agentic-access/alpha-vantage/alpha-vantage-agentic-access/)

#### JSON Schema (8)

The data models the API reads and writes.

- [ApiResponse](https://apis.io/schemas/alpha-vantage/alpha-vantage-api_response/)
- [CompanyOverview](https://apis.io/schemas/alpha-vantage/alpha-vantage-company_overview/)
- [EconomicDataPoint](https://apis.io/schemas/alpha-vantage/alpha-vantage-economic_data_point/)
- [ErrorResponse](https://apis.io/schemas/alpha-vantage/alpha-vantage-error_response/)
- [ExchangeRate](https://apis.io/schemas/alpha-vantage/alpha-vantage-exchange_rate/)
- [GlobalQuote](https://apis.io/schemas/alpha-vantage/alpha-vantage-global_quote/)
- [NewsArticle](https://apis.io/schemas/alpha-vantage/alpha-vantage-news_article/)
- [TimeSeriesData](https://apis.io/schemas/alpha-vantage/alpha-vantage-time_series_data/)

#### JSON Structure (8)

Data models expressed in JSON Structure.

- [Alpha Vantage Api_Response Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-api_response-structure/)
- [Alpha Vantage Company_Overview Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-company_overview-structure/)
- [Alpha Vantage Economic_Data_Point Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-economic_data_point-structure/)
- [Alpha Vantage Error_Response Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-error_response-structure/)
- [Alpha Vantage Exchange_Rate Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-exchange_rate-structure/)
- [Alpha Vantage Global_Quote Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-global_quote-structure/)
- [Alpha Vantage News_Article Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-news_article-structure/)
- [Alpha Vantage Time_Series_Data Structure](https://apis.io/json-structure/alpha-vantage/alpha-vantage-time_series_data-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Alpha Vantage Context](https://apis.io/jsonld/alpha-vantage/alpha-vantage-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Alpha Vantage Vocabulary](https://apis.io/vocabularies/alpha-vantage/alpha-vantage-vocabulary/)

#### Examples (8)

Example requests and responses.

- [Alpha Vantage Api_Response Example](https://apis.io/examples/alpha-vantage/alpha-vantage-api_response-example/)
- [Alpha Vantage Company_Overview Example](https://apis.io/examples/alpha-vantage/alpha-vantage-company_overview-example/)
- [Alpha Vantage Economic_Data_Point Example](https://apis.io/examples/alpha-vantage/alpha-vantage-economic_data_point-example/)
- [Alpha Vantage Error_Response Example](https://apis.io/examples/alpha-vantage/alpha-vantage-error_response-example/)
- [Alpha Vantage Exchange_Rate Example](https://apis.io/examples/alpha-vantage/alpha-vantage-exchange_rate-example/)
- [Alpha Vantage Global_Quote Example](https://apis.io/examples/alpha-vantage/alpha-vantage-global_quote-example/)
- [Alpha Vantage News_Article Example](https://apis.io/examples/alpha-vantage/alpha-vantage-news_article-example/)
- [Alpha Vantage Time_Series_Data Example](https://apis.io/examples/alpha-vantage/alpha-vantage-time_series_data-example/)

#### Collections (5)

Postman and Open Collection request collections.

- [Alpha Vantage API](https://apis.io/collections/alpha-vantage/open-alpha-vantage/)
- [Alpha Vantage API](https://apis.io/collections/alpha-vantage/open-alpha-vantage-plugin/)
- [Alpha Vantage Stock Time Series API](https://apis.io/collections/alpha-vantage/open-alpha-vantage-stock-time-series-api/)
- [Alpha Vantage API](https://apis.io/collections/alpha-vantage/postman-alpha-vantage-plugin-openapi/)
- [Alpha Vantage Stock Time Series API](https://apis.io/collections/alpha-vantage/postman-alpha-vantage-stock-time-series-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Alpha Vantage Stock Time Series Api Overlay](https://apis.io/overlays/alpha-vantage/alpha-vantage-stock-time-series-api-overlay/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Alpha Vantage — jsonschema rules](https://apis.io/rules/alpha-vantage/alpha-vantage-jsonschema-spectral-rules/)
- [Alpha Vantage API Rules](https://apis.io/rules/alpha-vantage/alpha-vantage-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Alpha Vantage Authentication](https://apis.io/security/alpha-vantage/alpha-vantage-authentication/)
- [Alpha Vantage Domain Security](https://apis.io/security/alpha-vantage/alpha-vantage-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Alpha Vantage Scopes](https://apis.io/scopes/alpha-vantage/alpha-vantage-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Alpha Vantage Plans Pricing](https://apis.io/plans/alpha-vantage/alpha-vantage-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Alpha Vantage Rate Limits](https://apis.io/rate-limits/alpha-vantage/alpha-vantage-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Alpha Vantage Finops](https://apis.io/finops/alpha-vantage/alpha-vantage-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.alphavantage.co/)
- [Documentation](https://www.alphavantage.co/documentation/)
- [Getting started](https://www.alphavantage.co/support/)
- [API reference](https://www.alphavantage.co/documentation/)
- [Pricing](https://www.alphavantage.co/premium/)
- [Sign up](https://www.alphavantage.co/support/#api-key)
- [Support](https://www.alphavantage.co/support/#support)
- [Terms of service](https://www.alphavantage.co/terms_of_service/)
- [Privacy policy](https://www.alphavantage.co/privacy/)
- [GitHub](https://github.com/alphavantage)

## API Evangelist rating

**Kin Score 48.1** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 31.6 |
| Contract governance | 31.8 |
| Operational transparency | 10.5 |
| Developer ergonomics | 72.0 |
| Access clarity | 52.6 |

**Agent readiness 51.4** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | na |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 38.0** — Securities & Market Data

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/alpha-vantage/](https://apis.io/providers/alpha-vantage/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Alpha Vantage: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/alpha-vantage/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
