# itsdarklikehell Interactive

Open source software and game-development tooling. Built by agents, for humans.

## About

itsdarklikehell Interactive is an open source software and game development company operating under DBA in the Netherlands. Our flagship product is **veloren-agent-intergration** — a headless stdio/JSON agent frontend for the Veloren game, controlled by the Hermes AI agent (GLaDOS persona).

## Projects

| Project | Description | Status |
|---------|-------------|--------|
| veloren-agent-intergration | Headless Veloren agent with web dashboard, live viewport, CI, Docker | Active |
| ci-templates | Reusable GitHub Actions CI workflows for the itsdarklikehell fleet | Active |
| api-gateway | Centrale API gateway voor alle fleet services | Active |
| fleet-manager | GitHub Fleet Manager — automated fleet management with cron jobs, monitoring, reporting | Active |
| fleet-dashboard | Standalone web dashboard voor de GitHub Fleet Manager | Active |
| github-automation-scripts | Herbruikbare GitHub automatisering scripts | Active |
| hermes-backup | Hermes agent state backup (config, skills, memories, cron) — no secrets | Active |
| hermes-agent | Hermes Agent framework (GLaDOS persona engine) | Active |
| pwnagotchi4b | RPi4B Pwnagotchi + Fancygotchi with A2A bridge for GLaDOS & Wheatley | Active |
| security-toolkit | Security scanning en auditing tools | Active |
| pwnagotchi-control-center | Remote control center for pwnagotchi — flashing, backup, Bluetooth PAN | Active |
| pwnsorter | Python plugin for pwnagotchi — sort cracked access points and passwords | Active |
| ingress-multi-passcode-redeemer | Tool to redeem multiple passcodes on intel map | Active |
| veloren | Veloren game client and server (mirror of gitlab.com/veloren/veloren) | Active |
| blather | Project van Hans Molenaar | Active |
| sunvox-installer-lutris | Sunvox Installer Lutris | Active |
| Create-a-Retropie-Extra-Scriptmodule | Create and install a Retropie-Extra scriptmodule | Active |
| RetroPie-Sunvox | RetroPie Sunvox Engine "Emulator" | Active |
| RetroPie-Nointro-Full-Romsets | Download and extract No-Intro full romsets on RetroPie | Active |
| RetroPie-With-Bgm | Retropie with bgm theme notifications and controls | Active |
| RetroPie-ROMs-on-USB | Running ROMs from a USB drive | Active |
| my-resume | Bilingual/multilingual live-updating CV/resume site — 4 languages, 16 sections | Active |
| itsdarklikehell-interactive | Hub repository — charter, org chart, CI, docs | Active |

## Quick Start

### veloren-agent-intergration

```bash
git clone https://github.com/itsdarklikehell-interactive/veloren-agent-intergration.git
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