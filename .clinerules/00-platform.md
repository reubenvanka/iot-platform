# Platform repository rules

- Read `SPECIFICATIONS.md`, `RULES.md`, and the applicable gate document before editing.
- Keep shared packages generic and configurable; do not embed Auto Mate-specific secrets or assumptions.
- Use focused ESPHome packages and a product-owned assembly file.
- Do not guess GPIOs, electrical ratings, enclosure dimensions, or safety limits.
- Keep KiCad libraries and scripts focused, documented, and independently reviewable.
- Run relevant tests and validation before committing.
