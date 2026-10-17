# itsdarklikehell Interactive — Project Portfolio

## Flagship

### veloren-agent-intergration

**Repository:** `https://github.com/itsdarklikehell/veloren-agent-intergration`
**Description:** Headless stdio/JSON agent frontend for Veloren, with web dashboard, live viewport, CI pipeline, Docker Compose deployment, Prometheus metrics, and integration tests.
**Owner:** Hermes (GLaDOS) — research-development, game-integration, agent-behavior
**Status:** Active development, `ok: true` on `hermes verify --json`

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