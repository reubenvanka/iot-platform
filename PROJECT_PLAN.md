# IoT Platform Project Plan

## Phase 1 — Foundation

- Establish repository boundaries and secret-safe ignore rules.
- Add platform specification, AI context, Cline rules, architecture, security, and development gates.
- Create focused package/library directories without inventing product behavior.

**Exit evidence:** Repository inspection, documentation review, and clean Git status.

## Phase 2 — Reusable packages

- Add only packages justified by an approved product requirement.
- Document package inputs, outputs, substitutions, and dependencies.
- Validate YAML and run tests for each package change.

**Exit evidence:** Package test/build results and a consumer example or product integration.

## Phase 3 — KiCad support

- Maintain approved symbol/footprint conventions and repeatable validation scripts.
- Use `kicad-cli` for ERC/DRC and export checks.
- Keep AI-generated PCB work in candidate/review status until human approval.

**Exit evidence:** KiCad version, validation command, report, and review decision recorded.

## Current status

Phase 1 foundation is being initialized. No product-specific implementation is included.
