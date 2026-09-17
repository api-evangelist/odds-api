---
name: Odds API line movement tracker
description: Track how a bookmaker's prices move for an event using Odds API snapshots and retained history.
api: Odds API REST
method: generated
operations:
  - list_events_events_get
  - odds_snapshot_events__event_id__odds_snapshot_get
  - odds_history_events__event_id__odds_history_get
---

# Line movement tracker

Base URL `https://api.odds-api.net/v1`; authenticate with `X-API-Key`.

## Steps

1. Discover events: `GET /events?sport=<sport>&league=<league>` (`list_events_events_get`), paging with `limit` + `cursor`.
2. Capture initial state: `GET /events/{event_id}/odds/snapshot` (`odds_snapshot_events__event_id__odds_snapshot_get`). Store `as_of_ts_ms` and any `resume` token.
3. Read retained movement: `GET /events/{event_id}/odds/history` (`odds_history_events__event_id__odds_history_get`) — returns `OddsHistorySeries` / `OddsHistoryPoint` for enabled accounts.
4. For live tracking, prefer the `/events/{event_id}/odds/stream` SSE feed (`sample_odds_stream` via MCP); apply `delta` messages idempotently and reconnect with `since=<last_resume>&catchup=true`.

## Rules

- History access is gated to enabled accounts / paid historical add-on; a `403` means the plan does not include it.
- A `413` on the odds snapshot means the requested breadth is too large — narrow markets/bookmakers.
- Watch `bookmaker_as_of_ts_ms` for per-bookmaker freshness; handle suspended selections.
- Errors follow `{ detail, code?, request_id? }`; honor `Retry-After` on `429`.
