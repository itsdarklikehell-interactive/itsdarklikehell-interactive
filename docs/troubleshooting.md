# Troubleshooting

## Agent Connection Issues

### Can't connect to server

**Symptoms:** Agent logs `ConnectionRefused` or `Connection timed out`.

**Causes:**
- Veloren server not running. Start it: `tmux attach -t veloren-server` or `docker compose up veloren-server`.
- Wrong port. Server listens on `14004` by default (`VELOREN_PORT`).
- Wrong host. In Docker Compose, use `veloren-server:14004`, not `127.0.0.1:14004`.

**Fix:**
```bash
ss -tlnp | grep 14004   # verify server is listening
```

### Presence never registers

**Symptoms:** Agent connects but `presence` stays `None` in `/api/viewport/latest`.

**Causes:**
- Character not found on server. Character name must match `VELOREN_AGENT_CHARACTER`.
- Authentication failed. Check `VELOREN_USERNAME` / `VELOREN_PASSWORD` in `.env`.
- Server in auth mode but credentials invalid for `auth.veloren.net`.

**Fix:**
- Verify character exists on the server.
- Verify credentials work against `https://auth.veloren.net`.

### Agent exits immediately

**Symptoms:** Agent process starts and exits with non-zero code.

**Causes:**
- Missing `VELOREN_ASSETS` — headless client needs Airshipper assets directory.
- Missing `veloren-server-cli` binary at `VELUREN_SERVER_BIN`.
- Rust compile errors. Run `cargo build --release -D warnings`.

### Dashboard can't start the agent

**Symptoms:** Dashboard reports missing agent binary.

**Causes:**
- `VELUREN_AGENT_BIN` points to wrong path.
- Release binary not built: `cargo build --release`.

### Docker Compose networking

**Symptoms:** Agent can't reach server inside Compose.

**Cause:** Services communicate via service name, not `localhost`.

**Fix:** Use `veloren-server:14004` inside the Compose network, not `127.0.0.1:14004`.

### No observations yet

**Symptoms:** `/api/viewport/latest` returns empty or stale data.

**Causes:**
- Agent not sending observations (connection lost).
- Dashboard not receiving (check `/api/health`).
- SQLite database missing at `.hermes/artifacts/dashboard.db`.

**Fix:**
- Restart agent and dashboard.
- Check agent logs: `docker compose logs veloren-agent` or `tmux attach -t veloren-server`.