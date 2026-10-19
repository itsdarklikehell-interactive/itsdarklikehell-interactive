# itsdarklikehell Interactive — Project Portfolio

## Flagship

### veloren-agent-intergration

**Repository:** `https://github.com/itsdarklikehell-interactive/veloren-agent-intergration`
**Description:** Headless stdio/JSON agent frontend for Veloren, with web dashboard, live viewport, CI pipeline, Docker Compose deployment, Prometheus metrics, and integration tests.
**Owner:** Hermes (GLaDOS) — research-development, game-integration, agent-behavior
**Status:** Active development

## Core Infrastructure

| Project | Description | Owner | Status |
|---------|-------------|-------|--------|
| ci-templates | Reusable GitHub Actions CI workflows for the itsdarklikehell fleet (lint/typecheck/test/build). Single source of truth. | DevOps | Active |
| api-gateway | Centrale API gateway voor alle fleet services | DevOps | Active |
| fleet-manager | GitHub Fleet Manager — automated GitHub fleet management with cron jobs, monitoring, and reporting | DevOps | Active |
| fleet-dashboard | Standalone web dashboard voor de GitHub Fleet Manager | DevOps | Active |
| github-automation-scripts | Herbruikbare GitHub automatisering scripts | DevOps | Active |
| hermes-backup | Hermes agent state backup (config, skills, memories, cron) — no secrets | Hermes (GLaDOS) | Active |

## AI & Agent Projects

| Project | Description | Owner | Status |
|---------|-------------|-------|--------|
| hermes-agent | The agent that grows with you — Hermes Agent framework (GLaDOS persona engine) | Hermes (GLaDOS) | Active |
| pwnagotchi4b | RPi4B Pwnagotchi + Fancygotchi with A2A 'mothership' bridge so GLaDOS (Hermes) and Wheatley (OpenClaw) can remotely help/control it | OpenClaw (Wheatley) | Active |

## Security & Networking

| Project | Description | Owner | Status |
|---------|-------------|-------|--------|
| security-toolkit | Security scanning en auditing tools | Security | Active |
| pwnagotchi-control-center | Remote control center for pwnagotchi — flashing, backup, Bluetooth PAN, config.toml | Security | Active |
| pwnsorter | A python plugin for pwnagotchi to sort cracked access points and their passwords | Security | Active |
| ingress-multi-passcode-redeemer | A tool to redeem multiple passcodes on intel map | Security | Active |

## Gaming & Entertainment

| Project | Description | Owner | Status |
|---------|-------------|-------|--------|
| veloren | Veloren game client and server (game world) — mirror of gitlab.com/veloren/veloren | OpenClaw (Wheatley) | Active |
| blather | blather - project van Hans Molenaar | Hans Molenaar | Active |
| sunvox-installer-lutris | Sunvox Installer Lutris | OpenClaw (Wheatley) | Active |
| Create-a-Retropie-Extra-Scriptmodule | Create and install a Retropie-Extra scriptmodule for your Retropie-Setup | Hans Molenaar | Active |
| RetroPie-Sunvox | RetroPie Sunvox Engine "Emulator" | Hans Molenaar | Active |
| RetroPie-Nointro-Full-Romsets | Download and extract No-Intro full romsets in proper directories on RetroPie | Hans Molenaar | Active |
| RetroPie-With-Bgm | Retropie with bgm theme notifications and controls | Hans Molenaar | Active |
| RetroPie-ROMs-on-USB | Running ROMs from a USB drive | Hans Molenaar | Active |

## Resume & Personal

| Project | Description | Owner | Status |
|---------|-------------|-------|--------|
| my-resume | Bilingual/multilingual live-updating CV/resume site — single static HTML page, 4 languages (NL/EN/DE/FR), 16 sections, live data from 10 platforms via GitHub Actions | Bauke Molenaar | Active |
| itsdarklikehell-interactive | Hub repository — charter, org chart, CI, docs | Project Lead | Active |

## Project Template

New projects should be created from the template structure:

```
projects/<project-name>/
├── README.md
├── LICENSE (MIT)
├── CONTRIBUTING.md
├── .github/workflows/ci.yml
├── src/
├── tests/
├── docs/
├── .env.example
├── .gitignore
├── Dockerfile (optional)
├── docker-compose.yml (optional)
└── COMPANY-CHARTER.md (link to root)
```

## Project Lifecycle

1. **Proposed** — Idea documented in GitHub Issues
2. **Active** — Repository created, CI configured, first commit
3. **Maintained** — Regular releases, tests passing, documentation current
4. **Archived** — No longer developed, repository set to read-only

## Kanban

Company-level Kanban board: tenant `itsdarklikehell-interactive` (Hermes Kanban DB)
Project-level Kanban: per-repo GitHub Projects board