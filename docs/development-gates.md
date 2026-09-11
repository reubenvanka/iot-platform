# Development Gates

## Gate 1 — Planning

**Entry:** An approved requirement or explicit product decision exists.

**Required evidence:**

- Updated `SPECIFICATIONS.md` with requirement IDs.
- Open questions and hardware TODOs recorded.
- Product impact identified for shared packages.

**Exit:** Planning review is recorded in the project plan.

## Gate 2 — Architecture

**Entry:** Planning gate passed.

**Required evidence:**

- Repository/component boundaries documented.
- Interfaces, substitutions, and data flow identified.
- Security and hardware-safety implications reviewed.

**Exit:** Architecture is recorded in `docs/architecture.md` and reviewed.

## Gate 3 — Implementation

**Entry:** Architecture gate passed.

**Required evidence:**

- Small change with focused tests or validation.
- No secrets or guessed hardware mapping.
- Documentation and changelog updated where behavior changes.

**Exit:** Relevant build, lint, test, or KiCad checks pass.

## Gate 4 — Release

**Entry:** Implementation and integration checks pass.

**Required evidence:**

- Requirement/test traceability complete.
- ERC/DRC or other applicable evidence recorded.
- Human approval for safety, connections, placement, routing, and release.

**Exit:** Release evidence is committed to `docs/release-evidence.md` and a tag is created only after approval.
