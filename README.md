# itsdarklikehell Interactive

Open source software and game-development tooling. Built by agents, for humans.

## About

itsdarklikehell Interactive is an open source software and game development company operating under DBA in the Netherlands. Our flagship product is **veloren-agent-intergration** — a headless stdio/JSON agent frontend for the Veloren game, controlled by the Hermes AI agent (GLaDOS persona). The organization maintains 100 repositories across AI agents, security tooling, gaming, RetroPie emulation, SDR radio, infrastructure, and personal projects.

## Projects (All 42 Own Repositories)

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
| pwnagotchi-control-center | Remote control center for pwnagotchi — flashing, backup, Bluetooth PAN | Active |
| pwnsorter | Python plugin for pwnagotchi — sort cracked access points and passwords | Active |
| pwnspeaker | Python plugin for pwnagotchi TTS | Active |
| apprise-notify | Plugin for pwnagotchi that uses apprise to send notifications | Active |
| pwnagotchi-plugins | Collectie van Pwnagotchi-plugins voor Wi-Fi auditing en pentesting | Active |
| pwnagotchijay | Raspberry Pi instrumenting Bettercap for Wi-Fi pwning | Active |
| pwnmothership | Project van Hans Molenaar | Active |
| security-toolkit | Security scanning en auditing tools | Active |
| ingress-multi-passcode-redeemer | Tool to redeem multiple passcodes on intel map | Active |
| AngryOxide | 802.11 Attack Tool | Active |
| veloren | Veloren game client and server (mirror of gitlab.com/veloren/veloren) | Active |
| blather | Project van Hans Molenaar | Active |
| sunvox-installer-lutris | Sunvox Installer Lutris | Active |
| Create-a-Retropie-Extra-Scriptmodule | Create and install a Retropie-Extra scriptmodule | Active |
| RetroPie-Sunvox | RetroPie Sunvox Engine "Emulator" | Active |
| RetroPie-Nointro-Full-Romsets | Download and extract No-Intro full romsets on RetroPie | Active |
| RetroPie-With-Bgm | Retropie with bgm theme notifications and controls | Active |
| RetroPie-ROMs-on-USB | Running ROMs from a USB drive | Active |
| pokemon-agent | Pokemon-playing agent | Experimental |
| airi | Self hosted Grok Companion — realtime voice chat, Minecraft, Factorio | Active |
| raspbian-installer | Download, unzip, burn and modify a raspbian version to a device | Active |
| raspbian-after-burner | raspbian-after-burner - project van Hans Molenaar | Active |
| picoTracker | picoTracker - project van Hans Molenaar | Active |
| picoTracker-Theme-Studio | picoTracker Theme Studio | Active |
| tv-control | Control TV over HDMI (cec-client) | Active |
| stonetop-wiki-generator | Generate a static wiki from the Stonetop Book PDFs | Active |
| Open-LLM-VTuber | Talk to any LLM with hands-free voice, voice interruption, Live2D face | Experimental |
| avoid-ai-writing | Skill that audits and rewrites content to remove AI writing patterns | Active |
| ccusage | npx ccusage | Active |
| clawhub | Skill + Plugin Registry for OpenClaw | Active |
| Domo-Installer | Domo-Installer - project van Hans Molenaar | Active |
| rtorrent | rTorrent BitTorrent client | Active |
| ProxmoxVE | Proxmox VE Helper-Scripts (Community Edition) | Active |
| PVE-mods | Proxmox modifications | Active |
| foundryvtt-docker | Easy-to-deploy containerized Foundry Virtual Tabletop server | Active |
| charnik-content-srd | SRD D&D 5.1.0 and SRD D&D 5.2.1 for Charnik | Active |
| autocontext | Recursive self-improving harness for agents | Active |
| the-good-bits | Auto audio sample chopper and extractor | Active |
| dice | Compute dice rolls according to RPG dice notation | Active |
| skills-getting-started-with-github-copilot | Exercise: Get started using GitHub Copilot | Active |
| my-resume | Bilingual/multilingual live-updating CV/resume site — 4 languages, 16 sections | Active |
| itsdarklikehell-interactive | Hub repository — charter, org chart, CI, docs | Active |
| omarchy-config | Omarchy configuration synced by omarsync | Active |
| omarchy-configs | Omarchy configurations | Active |
| omarchy-dotfiles | Per-host Omarchy dotfiles (chezmoi) — desktop + laptop | Active |
| batch_comfytester-stub | Batch Civitai/ComfyUI model tester stub | Active |
| batch_comfytester | Batch Civitai/ComfyUI model tester stub | Active |

## Private Repositories (5)

| Repo | Description |
|------|-------------|
| omarchy-config | Omarchy configuration synced by omarsync |
| omarchy-configs | Omarchy configurations |
| omarchy-dotfiles | Per-host Omarchy dotfiles (chezmoi) — desktop + laptop |
| hermes-backup | Hermes agent state backup (config, skills, memories, cron) — no secrets |
| batch_comfytester | Batch Civitai/ComfyUI model tester stub |

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