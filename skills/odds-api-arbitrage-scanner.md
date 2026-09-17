---
name: Odds API arbitrage scanner
description: Find cross-bookmaker arbitrage opportunities from the Odds API betting-opportunity snapshot feed.
api: Odds API REST
method: generated
operations:
  - snapshot_bets_snapshot_get
  - bookmakers_bookmakers_get
  - get_event_events__event_id__get
---

# Arbitrage scanner

Grounded in real Odds API V1 operations. Base URL `https://api.odds-api.net/v1`; send `X-API-Key` on every request.

## Steps

1. (Optional) Discover available bookmakers with `GET /bookmakers` (`bookmakers_bookmakers_get`) to confirm coverage for your account tier.
2. Pull the arbitrage feed: `GET /bets/snapshot?strategies=arbitrage` (`snapshot_bets_snapshot_get`). Each `BetOpportunity` carries `event_id`, `bookmaker_name`, `selection_key`, and the implied edge.
3. For any opportunity, fetch event context with `GET /events/{event_id}` (`get_event_events__event_id__get`) to confirm start time, event_state, and that selections are not suspended.
4. Respect the per-tier bookmaker limit for bets feeds (2 / 6 / 15 / 50 by plan) — opportunities are computed only across bookmakers your plan enables.

## Rules

- Never describe arbitrage as guaranteed profit; account for execution risk, stake limits, and price movement before display or action.
- Check `as_of_ts_ms` / `bookmaker_as_of_ts_ms` freshness and handle suspended selections and empty arrays.
- Handle `429` by honoring `Retry-After`; poll betting-opportunity snapshots no faster than every 30–120s unless streaming.
- Errors follow `{ detail, code?, request_id? }` (not RFC 9457) — see errors/odds-api-problem-types.yml.
