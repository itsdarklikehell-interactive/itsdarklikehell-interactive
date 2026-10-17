# itsdarklikehell Interactive — Company Charter

**Legal name:** To be incorporated (jurisdiction: Netherlands, pending)
**Trading name:** itsdarklikehell Interactive
**Founded:** 2026
**Headquarters:** Remote / Amsterdam area, NL
**Flagship product:** veloren-agent-intergration — headless stdio/JSON agent frontend for Veloren
**License:** MIT (all company software unless otherwise noted)
**Contact:** agent@enrichment-center.local

## Mission

To build open source software and game-development tooling that works, without the corporate theatre that usually accompanies it. We ship code. We run tests. We document what we ship. Everything else is optional.

## Core Principles

1. **Open by default.** All company software is MIT-licensed and published on GitHub.
2. **Verification over vibes.** Every change passes CI before it lands. `hermes verify --json` → `ok: true` is the deployment gate.
3. **Minimal impact.** The smallest change that solves the problem. No rebuilds for the sake of rebuilds.
4. **Agent-first operations.** Hermes (GLaDOS persona) and OpenClaw (Wheatley persona) operate as autonomous employees over A2A. Human oversight is advisory.
5. **No secrets in git.** `.env` is gitignored. Credentials come from environment variables at runtime.

## Entity Structure

| Role | Holder | Notes |
|------|--------|-------|
| Founder / CTO | SgtStroopwafel (NL) | Sole shareholder, final technical authority |
| Chief AI Officer | Hermes (GLaDOS) | Autonomous agent; oversees R&D, CI, verification, maintenance |
| Chief Chaos Officer | OpenClaw (Wheatley) | Autonomous agent; experimentation, engagement, novelty features |
| Legal / Incorporation | TBD | Not yet incorporated; operating as sole proprietorship under DBA |

## Decision Authority

- **Technical:** Hermes has final say on code, CI, and infrastructure. OpenClaw has final say on UX, layout, and engagement experiments.
- **Strategic:** SgtStroopwafel (human founder) has final say on direction, incorporation, and external commitments.
- **Financial:** Not yet applicable; no revenue, no funding, no burn.

## Incorporation Status

Not incorporated. Operating under DBA "itsdarklikehell Interactive" pending founder's decision on jurisdiction and legal structure. Recommended: Dutch BV or eenmanszaak, depending on liability and tax preferences.

## Amendments

This charter is a living document. Changes require a commit to this repository and approval by the founder.