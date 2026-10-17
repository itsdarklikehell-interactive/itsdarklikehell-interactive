# Veloren Agent Deploy Runbook

## Overview

Deploy the veloren-agent headless game agent with web dashboard and live viewport using Docker Compose.

## Services

| Service | Image | Ports | Purpose |
|---------|-------|-------|---------|
| veloren-server | rust:1.99 + nightly | 14004 | Veloren dedicated server |
| veloren-agent | rust:1.99 + nightly | (internal) | Headless game agent |
| veloren-dashboard | Flask dashboard | 5000 | Web dashboard + live viewport |

## Prerequisites

- Docker + Docker Compose v2
- `.env` file with `VELOREN_USERNAME`, `VELOREN_PASSWORD`, `DASHBOARD_API_KEY`
- Airshipper assets at `VELOREN_ASSETS` (for headless client)

## Quick Start

```bash
cp .env.example .env
# Edit .env with your credentials
docker compose config          # validate
docker compose up --build      # build and start
```

## Verify

```bash
curl http://127.0.0.1:5000/api/health          # 200 OK
curl http://127.0.0.1:5000/viewport            # 200 OK (live viewport)
curl http://127.0.0.1:5000/api/viewport/latest # agent observation JSON
```

Open `http://127.0.0.1:5000/viewport` in your browser.

## Stop

```bash
docker compose down
```

## Production Notes

- Place a TLS reverse proxy (nginx, caddy, traefik) in front of the dashboard.
- The Flask dev server is not production-grade; use gunicorn for public-facing deployments.
- Never commit `.env`. It is gitignored.
- API key required on all endpoints except `/`, `/api/health`, `/metrics`, `/viewport`, `/api/viewport/*`.

## Build Notes / Known Fixes

- `veloren-client`, `veloren-common`, `veloren-common-net` pinned to same git rev (`f97be347...`) to prevent duplicate crate instances and `ControllerInputs` type mismatches.
- `shred` patch: `core::ptr::invalid_mut` → `wrapping_add().cast()` for newer nightly Rust.
- `foldhash`, `hashbrown`, `vek`: nightly feature gates patched out for stability.
- `docker compose build veloren-agent` verified: all tests pass, image builds clean.