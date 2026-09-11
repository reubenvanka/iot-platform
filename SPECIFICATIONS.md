# IoT Platform Specification

**Status:** Foundation specification

**Source of truth:** This file. Architecture and implementation must not introduce behavior that conflicts with it.

## Scope

The platform provides shared, reusable infrastructure for ESPHome products and KiCad-assisted hardware development. It does not define product-specific GPIO mappings, credentials, customer data, or release approvals.

## Requirements

| ID | Requirement | Acceptance evidence |
| --- | --- | --- |
| PLAT-REQ-001 | Provide focused ESPHome packages under `esphome/packages/` for behavior shared by multiple products. | Package files are documented and consumed by a product assembly file. |
| PLAT-REQ-002 | Keep secrets and credentials outside Git and provide secret-safe configuration guidance. | `.gitignore`, documentation, and repository inspection show no committed secrets. |
| PLAT-REQ-003 | Support KiCad 10 project validation through `kicad-cli` and documented human-review gates. | KiCad version and validation commands are recorded in release evidence. |
| PLAT-REQ-004 | Maintain persistent AI rules and derived context documentation in each repository. | `.clinerules/`, `docs/ai-context.md`, and `SPECIFICATIONS.md` are present. |
| PLAT-REQ-005 | Keep platform and product repositories independently versioned. | Each repository has its own Git history and no product is committed into the platform repository. |
| PLAT-REQ-006 | Require explicit hardware mapping before GPIO-dependent implementation. | TODOs or approved hardware files identify every used GPIO. |

## Non-goals

- Replacing product specifications with platform defaults.
- Guessing pin assignments, electrical ratings, or safety requirements.
- Making AI-generated KiCad output automatically manufacturing-ready.
- Storing production credentials or private customer data.

## Change control

Behavioral changes require a specification update, requirement/test IDs where applicable, and a review of affected documentation and tests. Breaking package changes require a migration note and product impact review.
