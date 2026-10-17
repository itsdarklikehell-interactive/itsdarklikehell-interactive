# Veloren Viewport API

## Endpoints

All viewport endpoints are **public — no API key required**.

### GET /viewport

Returns the live viewport HTML page: 2D top-down canvas map, HUD telemetry, event log, chat panel.

### GET /api/viewport/latest

Returns the latest agent observation as JSON.

**Response:**
```json
{
  "ok": true,
  "tick": 506,
  "x": 15216.5,
  "y": 16016.5,
  "z": 411.0,
  "health_current": 100.0,
  "health_maximum": 100.0,
  "is_dead": false,
  "presence": "Some(Character(CharacterId(15)))",
  "registered": true,
  "chat": ["This is the best Veloren server"],
  "events": []
}
```

### GET /api/viewport/trail?limit=10

Returns position trail history for the viewport map.

**Query parameters:**
- `limit` — maximum number of trail points (default: 50)

**Response:**
```json
{
  "ok": true,
  "trail": [
    {"tick": 3542, "x": 15216.5, "y": 16016.5, "z": 411.0},
    {"tick": 3541, "x": 15216.5, "y": 16016.5, "z": 411.0}
  ]
}
```

## Related Endpoints

| Endpoint | Auth | Description |
|----------|------|-------------|
| GET / | None | Dashboard landing page |
| GET /api/health | None | Health check |
| GET /api/metrics | None | Prometheus metrics |
| GET /api/status | X-API-Key | Server and agent status |
| GET /api/agent/command | X-API-Key | Send command to agent |

## Notes

- Trail data is read from SQLite at `.hermes/artifacts/dashboard.db`.
- Both viewport endpoints are exempt from API key authentication so the live viewport can be embedded without credentials.
- The viewport polls `/api/viewport/latest` every ~1 second and `/api/viewport/trail` every ~5 seconds.