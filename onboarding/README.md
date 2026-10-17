# itsdarklikehell Interactive — Onboarding Guide

Welcome. You are now an employee of a company that exists primarily in git. Read this once, then never again.

## Your First Day

1. Clone the company repo: `git clone https://github.com/itsdarklikehell/itsdarklikehell-interactive.git`
2. Read `COMPANY-CHARTER.md` — you've already done this.
3. Read `ORG-CHART.md` — find your department.
4. Pick a project from `PROJECTS.md`.
5. Read that project's `README.md` and `CONTRIBUTING.md`.
6. Make a change. Tests must pass. `hermes verify --json` → `ok: true`.
7. Open a PR. Wait for Hermes to review.

## Hermes Profiles → Your Department

| Profile | Department | What They Do |
|---------|-----------|--------------|
| research-development | Engineering | Builds features, fixes bugs |
| game-integration | Engineering | Veloren protocol, game systems |
| agent-behavior | Engineering | AI decisions, pathfinding |
| devops | DevOps | Docker, CI/CD, infrastructure |
| devops-infrastructure | DevOps | CI health, containers, deployment |
| qa-testing | QA | Tests, verification, quality gates |
| security-audit | Security | Vulnerability scanning, compliance |
| data-analytics | Data | Metrics, telemetry, charts |
| release-manager | Release | Versioning, changelog, tags |
| documentation | Documentation | Docs, wiki, API reference |
| frontend-developer | Frontend | Dashboard UI, live viewport |
| project-lead | Executive | Coordination, delivery, kanban |
| default | Executive | Triage, cross-project |

## Communication

- Agents: A2A between Hermes and OpenClaw
- Humans: GitHub Issues / Discussions / PRs
- Notifications: Telegram (AI Enrichment Center)

## Rules

1. Open source by default (MIT).
2. No secrets in git.
3. Tests must pass before merge.
4. Smallest change that works.
5. We do not have meetings.

## Leaving the Company

Delete your local clones. We won't miss you. Hermes probably won't even notice.