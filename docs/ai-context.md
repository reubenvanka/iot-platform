# IoT Platform AI Context

## Purpose

This repository supports reusable ESPHome packages, KiCad libraries, automation scripts, and cross-product documentation. It does not contain Auto Mate product secrets or guessed hardware mappings.

## Current toolchain

- KiCad 10.0.6 at `/Applications/KiCad/KiCad.app`
- `kicad-cli` at `/opt/homebrew/bin/kicad-cli`
- MCP server source at `/Users/reubenvanka/Desktop/kicad-mcp-server`
- Modern Python at `/opt/homebrew/bin/python3`
- KiCad bundled Python at `/Applications/KiCad/KiCad.app/Contents/Frameworks/Python.framework/Versions/3.9/bin/python3`

## Operating boundary

Use AI for candidate generation, parsing, validation reports, and documentation assistance. The modern-Python MCP server startup, 45-tool registry, project creation, PCB outline setup, ERC, and DRC workflow are validated. Do not treat generated KiCad output as approved hardware, and do not infer GPIOs or electrical ratings from a symbol name alone.
