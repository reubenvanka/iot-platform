# Release Evidence

This file is the release evidence index for the platform repository.

## Current foundation release

- Date: 2026-09-11
- Scope: Repository foundation, source-of-truth documentation, AI rules, secret-safe ignore policy, and development gates.
- KiCad CLI: `kicad-cli --version` → `10.0.6`
- MCP environment: `/Users/reubenvanka/.local/share/iot-tools/kicad-mcp-venv/bin/python` → Python 3.14.7
- MCP dependencies: installed from `/Users/reubenvanka/Desktop/kicad-mcp-server/requirements.txt`
- MCP startup: stdio server startup completed successfully with `show_banner=False`.
- MCP registry: 45 tools registered, including project creation, PCB setup, ERC, and DRC.
- MCP smoke workflow: temporary KiCad project creation succeeded; 50 × 40 mm PCB outline setup succeeded; ERC passed; DRC passed.
- Cline MCP settings: command and environment verified; `KICAD_CLI` is pinned to `/opt/homebrew/bin/kicad-cli`.
- GitHub CLI: `gh` 2.100.0 installed; browser authentication is pending, so no remotes or pushes have been created.
- Product code: None included in this repository.
- Human release approval: Pending; this is a foundation commit, not a product release.

## Evidence checklist

- [x] Repository inspection completed.
- [x] No secrets or credentials committed.
- [x] Relevant MCP and KiCad validation commands recorded.
- [ ] Human review completed for any hardware-related release.

## Validation boundary

The text-parser and CLI-backed MCP workflow is validated. KiCad's bundled `pcbnew` Python bindings remain tied to Python 3.9, so API-backed PCB editing still requires a separately verified bridge or compatible server. Candidate KiCad output remains subject to human electrical and manufacturing review.
