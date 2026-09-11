# IoT Platform

Shared infrastructure for ESPHome products and KiCad-assisted hardware workflows.

## Scope

This repository owns reusable platform packages, KiCad library conventions, automation scripts, and cross-product development rules. Product-specific requirements and product assembly files belong in the product repository that consumes this platform.

## Layout

- `esphome/packages/` — reusable ESPHome packages.
- `kicad/symbols/` — approved project symbol libraries.
- `kicad/footprints/` — approved project footprint libraries.
- `scripts/` — repeatable validation and project-support scripts.
- `tests/` — platform-level tests and fixtures.
- `docs/` — architecture, workflow, security, and AI context.
- `.clinerules/` — persistent Cline instructions for this repository.

## Rules

`SPECIFICATIONS.md` is the source of truth. Read `RULES.md` and `docs/development-gates.md` before changing behavior. Do not add product secrets or customer data to this repository.

## Validation

Use the repository's relevant package, lint, test, and KiCad CLI checks. Record release evidence in `docs/release-evidence.md`.
