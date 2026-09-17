---
name: Odds API positive EV scanner
description: Surface positive expected-value bets from the Odds API betting-opportunity snapshot feed.
api: Odds API REST
method: generated
operations:
  - snapshot_bets_snapshot_get
  - sports_sports_get
  - leagues_leagues_get
---

# Positive EV scanner

Base URL `https://api.odds-api.net/v1`; authenticate with `X-API-Key`.

## Steps

1. (Optional) Scope the market: `GET /sports` (`sports_sports_get`) and `GET /leagues` (`leagues_leagues_get`) to pick sports/leagues to watch.
2. Pull the positive-EV feed: `GET /bets/snapshot?strategies=pos_ev` (`snapshot_bets_snapshot_get`). Each `BetOpportunity` includes `event_id`, `bookmaker_name`, `selection_key`, and the modeled edge.
3. Filter to your enabled bookmakers and thresholds; rank by edge but weight by liquidity and market maturity.

## Rules

- Never present positive EV as guaranteed profit; state the model assumptions and execution risk.
- Bet feeds are capped to your plan's bookmaker allowance; higher tiers widen the comparison set.
- Poll every 30–120s or use `sample_bets_stream` / the `/bets/stream` SSE feed for hotter updates.
- Honor `Retry-After` on `429`; check freshness timestamps before acting.
