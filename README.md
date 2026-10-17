# itsdarklikehell Interactive

Open source software and game-development tooling. Built by agents, for humans.

## About

itsdarklikehell Interactive is an open source software and game development company operating under DBA in the Netherlands. Our flagship product is **veloren-agent-intergration** — a headless stdio/JSON agent frontend for the Veloren game, controlled by the Hermes AI agent (GLaDOS persona).

## Projects

| Project | Description | Status |
|---------|-------------|--------|
| veloren-agent-intergration | Headless Veloren agent with web dashboard, live viewport, CI, Docker | Active |
| (template) | New project template | Planned |

## Quick Start

### veloren-agent-intergration

```bash
git clone https://github.com/itsdarklikehell/veloren-agent-intergration.git
cd veloren-agent-intergration
cp .env.example .env
# Fill in VELOREN_USERNAME and VELOREN_PASSWORD in .env
cargo build --release
./target/release/veloren-agent --character hermes
```

Then open `http://127.0.0.1:5000/viewport` in your browser to watch the agent play live.

## Company Documents

- [Company Charter](./COMPANY-CHARTER.md) — Mission, principles, decision authority
- [Org Chart](./ORG-CHART.md) — Department mapping, Hermes profiles → roles
- [Contributing](./CONTRIBUTING.md) — How to contribute
- [Code of Conduct](./CODE_OF_CONDUCT.md) — Community standards
- [Security](./SECURITY.md) — Vulnerability reporting

## License

MIT. See [LICENSE](./LICENSE).

## Contact

agent@enrichment-center.local