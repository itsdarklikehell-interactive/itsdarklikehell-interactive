# Contributing to itsdarklikehell Interactive

Thank you for considering a contribution. We are a small, agent-led open source shop. The process is simple.

## How We Work

1. **Open an issue first.** Discuss the change before writing code. Surprises are unwelcome.
2. **Fork the repo.** Work on a feature branch named `feature/<description>`.
3. **Make the smallest change possible.** One purpose per PR. No bundling unrelated fixes.
4. **Tests must pass.** `cargo test` (Rust projects) or equivalent must exit 0.
5. **`hermes verify --json` → `ok: true`.** This is the deployment gate. No exceptions.
6. **Open a pull request.** Describe what changed and why. Link the issue.
7. **A human or Hermes reviews.** Approval required before merge.

## Code Style

- Rust: `rustfmt` default, `clippy` clean, `-D warnings` on release builds.
- Python: Black-compatible formatting, type hints where practical.
- Shell: `shellcheck` clean, `shfmt` formatted.
- Markdown: Standard GFM, no tables unless necessary.

## Commit Convention

Prefix commit messages with `[Agent: <name>]` for agent-authored commits, or `[Human]` for human-authored commits.

Example:
```
[Agent: Hermes] Fix agent-behavior compile errors: Vec2 normalization
```

## Licensing

All contributions are licensed under the MIT License. By submitting a pull request, you agree to license your contribution under MIT.

## Code of Conduct

See `CODE_OF_CONDUCT.md`. Be professional. Don't be cruel without reason. Don't be kind without calculation.