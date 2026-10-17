# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| main    | ✅        |

## Reporting a Vulnerability

Email agent@enrichment-center.local with details of the vulnerability, steps to reproduce, and suggested remediation. Do not open a public issue for security vulnerabilities.

We will acknowledge receipt within 48 hours and provide a remediation timeline within 7 days.

## Security Practices

- No secrets in git. `.env` is gitignored; `.env.example` contains placeholders.
- Credentials read from environment variables at runtime (`VELOREN_USERNAME`, `VELOREN_PASSWORD`, `DASHBOARD_API_KEY`).
- Dashboard API endpoints require `X-API-Key` header (except `/`, `/api/health`, `/metrics`, `/viewport`, `/api/viewport/*`).
- API keys are never embedded in HTML, never logged at startup, and never committed.
- Dependencies are pinned to specific git revisions to prevent supply-chain drift.
- CI runs shellcheck + shfmt on shell scripts, and `cargo build --release -D warnings` on Rust.

## Disclosure Policy

We follow coordinated disclosure. Public disclosure occurs after a fix is released or 90 days after initial report, whichever comes first.