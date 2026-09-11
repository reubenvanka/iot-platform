# IoT Platform Architecture

**Source:** `SPECIFICATIONS.md` — update the specification before changing architecture.

## Repository boundary

The platform repository contains reusable infrastructure only. Product-specific requirements, credentials, GPIO mappings, and release decisions remain in the consuming product repository.

## ESPHome package model

- Shared behavior belongs in focused YAML packages under `esphome/packages/`.
- A product assembly file imports only the packages it needs.
- Package inputs should use substitutions or IDs rather than hard-coded product names.
- A package change must include a consumer impact review and relevant validation.

## KiCad library model

- Approved project symbols and footprints are stored under `kicad/`.
- Library additions require a source, license/usage note, and review.
- Generated or temporary KiCad outputs are excluded from Git.

## Validation model

- Use `kicad-cli` for schematic, PCB, ERC, DRC, and export checks where applicable.
- Text parsing is acceptable for candidate analysis when `pcbnew` is unavailable.
- Human review is mandatory before electrical or manufacturing decisions.
