# Odds API

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

OpenAPI-first sports betting odds API (odds-api.net) providing bookmaker odds, odds comparison, arbitrage, positive EV, line movement, and racing/sports coverage via REST plus SSE and WebSocket streaming. Agent-native with an MCP server, llms.txt, and agent instruction files, plus TypeScript and Python SDKs.

**Areas:** Sports · Sports Betting · betting-odds · bookmaker-odds · live-odds · Sportsbook · Racing · REST · Server-Sent Events · WebSocket · OpenAPI · MCP

## Odds API on APIs.io

Everything profiled for Odds API is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/odds-api/](https://apis.io/providers/odds-api/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [Odds API Account API](https://apis.io/apis/odds-api/odds-api-account-api/) — Current API identity, usage counters, and contract limits.
- [Odds API Betting opportunities API](https://apis.io/apis/odds-api/odds-api-betting-opportunities-api/) — Positive EV, arbitrage, middle, and bonus-bet opportunity feeds.
- [Odds API Catalog API](https://apis.io/apis/odds-api/odds-api-catalog-api/) — Supported sports, leagues, bookmakers, and approximate market coverage.
- [Odds API Prediction markets API](https://apis.io/apis/odds-api/odds-api-prediction-markets-api/) — Event-linked prediction-market order books with probability ladders, liquidity, and live updates.
- [Odds API Racing events API](https://apis.io/apis/odds-api/odds-api-racing-events-api/) — Racing event discovery and live racing event updates.
- [Odds API Racing odds API](https://apis.io/apis/odds-api/odds-api-racing-odds-api/) — Racing odds snapshots, home racing feeds, Server-Sent Events, and WebSocket updates.
- [Odds API Results API](https://apis.io/apis/odds-api/odds-api-results-api/) — Sports event result lookup.
- [Odds API Sports events API](https://apis.io/apis/odds-api/odds-api-sports-events-api/) — Upcoming and live sports events plus event metadata.
- [Odds API Sports exchange API](https://apis.io/apis/odds-api/odds-api-sports-exchange-api/) — Sports betting exchange order books with back/lay ladders, liquidity, and live updates.
- [Odds API Sports odds API](https://apis.io/apis/odds-api/odds-api-sports-odds-api/) — Sports odds snapshots, line movement, Server-Sent Events, and WebSocket updates.
- [Odds API Start here API](https://apis.io/apis/odds-api/odds-api-start-here-api/) — API identity, base URL, authentication, and reference links.
- [Odds API Status API](https://apis.io/apis/odds-api/odds-api-status-api/) — Buyer-facing API availability, latency, stream health, and rate-limit health.
- [Odds API Widgets API](https://apis.io/apis/odds-api/odds-api-widgets-api/) — Public-safe embeddable widget feeds for approved API clients.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Odds API MCP Server](https://apis.io/servers/odds-api/odds-api-mcp-server/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Odds Api Overlay](https://apis.io/overlays/odds-api/odds-api-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Odds Api Authentication](https://apis.io/security/odds-api/odds-api-authentication/)
- [Odds Api Domain Security](https://apis.io/security/odds-api/odds-api-domain-security/)
- [Odds Api Vulnerability Disclosure](https://apis.io/security/odds-api/odds-api-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Odds Api Plans Pricing](https://apis.io/plans/odds-api/odds-api-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Odds Api Rate Limits](https://apis.io/rate-limits/odds-api/odds-api-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://odds-api.net/)
- [Pricing](https://odds-api.net/pricing)
- [Terms of service](https://odds-api.net/terms)
- [Privacy policy](https://odds-api.net/privacy)
- [GitHub](https://github.com/odds-api)

## API Evangelist rating

**Kin Score 58.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 52.1 |
| Contract governance | 4.5 |
| Operational transparency | 60.5 |
| Developer ergonomics | 63.6 |
| Access clarity | 76.3 |

**Agent readiness 45.5** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | na |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | unknown |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/odds-api/](https://apis.io/providers/odds-api/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Odds API: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/odds-api/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
