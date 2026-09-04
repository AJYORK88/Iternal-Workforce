# Iternal Workforce

Senior design project for the Iternal Workforce initiative.

## Repository layout

| Path | Purpose |
|---|---|
| `documentation/` | All project docs. Order of authority: `requirements.md` → `documentation/design/*` → `documentation/agent-coordination/*`. |
| `documentation/design/` | Numbered architecture/design docs — the build spec. |
| `documentation/design-review/` | Red-team / design-review reports against the docs. |
| `documentation/design-system/` | Tokens, components, and static UI mockups. |
| `documentation/agent-coordination/` | Phase plan and file-ownership matrix. |
| `documentation/features/` | Implementation-free feature writeups (indexed in its README). |
| `documentation/research/` | Background research and references. |
| `documentation/code-review/` | Code-review findings and remediation status. |
| `documentation/UI-verification/` | Dated UI review reports. |
| `documentation/tests/` | Unit-test checklists. |
| `documentation/dev-guides/` | Setup, deploy, and troubleshooting runbooks. |
| `documentation/handoffs/` | Dated session-handoff notes. |
| `src/` | Application source (`api`, `auth`, `db`, `features`, `lib`, `types`, `ui`). |
| `tests/` | Automated tests mirroring `src/`. |
| `migrations/` | Numbered, additive-only DB migrations. |
| `scripts/` | Seed data and operational scripts. |
| `resources/` | Non-code assets (logos, reference files, sample data). |

Each folder contains a `README.md` describing what belongs there.

## Conventions

- Component architecture; no monoliths. Feature-specific code lives in `src/features/<feature>/`.
- All SQL lives in `src/db/`. Migrations are additive-only.
- Every commit passes typecheck and the full test suite.
- Significant actions are appended to `CHANGELOG.md`.
