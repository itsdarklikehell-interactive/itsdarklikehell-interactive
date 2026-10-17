# itsdarklikehell Interactive — Project Portfolio

## Flagship

### veloren-agent-intergration

**Repository:** `https://github.com/itsdarklikehell/veloren-agent-intergration`
**Description:** Headless stdio/JSON agent frontend for Veloren, with web dashboard, live viewport, CI pipeline, Docker Compose deployment, Prometheus metrics, and integration tests.
**Owner:** Hermes (GLaDOS) — research-development, game-integration, agent-behavior
**Status:** Active development, `ok: true` on `hermes verify --json`

## Company Projects (submodules)

| Project | Description | Owner | Status |
|---------|-------------|-------|--------|
| veloren-agent-intergration | Headless Veloren agent with web dashboard, live viewport, CI, Docker | Hermes (GLaDOS) | Active |
| veloren | Veloren game client and server (game world) | OpenClaw (Wheatley) | Active |
| teloren | Headless Veloren frontend reference architecture | Hermes (GLaDOS) | Reference |
| airshipper | Veloren asset and server distribution manager | DevOps | Active |
| hermes-agent | Hermes Agent framework (GLaDOS persona engine) | Hermes (GLaDOS) | Active |
| hermes-skills | Hermes skill library | Hermes (GLaDOS) | Active |
| ci-templates | Shared CI shell templates (shellcheck + shfmt) | DevOps | Active |
| ComfyUI-Installer | ComfyUI installation and setup tooling | OpenClaw (Wheatley) | Active |
| SwarmUI | SwarmUI interface tooling | OpenClaw (Wheatley) | Active |
| OpenClaw-bot-review | OpenClaw bot code review automation | OpenClaw (Wheatley) | Active |
| openclaw-office | OpenClaw office productivity tools | OpenClaw (Wheatley) | Active |
| GLaDOS-TTS | GLaDOS voice synthesis (Piper TTS voices) | Hermes (GLaDOS) | Active |
| hermes-desktop | Hermes desktop application | Hermes (GLaDOS) | Active |
| hermes-webui | Hermes web user interface | Hermes (GLaDOS) | Active |
| pokemon-agent | Pokemon-playing agent | Hermes (GLaDOS) | Experimental |
| agent-of-empires | Age of Empires agent | Hermes (GLaDOS) | Experimental |

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