# KiCad Workflow

## Supported workflow

1. Create or inspect a KiCad project skeleton.
2. Add approved symbols and candidate connections.
3. Export and inspect the netlist.
4. Establish a candidate PCB outline and initial placement.
5. Run `kicad-cli` ERC/DRC checks and review the report.
6. Require human approval for final connections, placement, routing, safety, and release.

## Local tools

- KiCad: `/Applications/KiCad/KiCad.app`
- CLI: `/opt/homebrew/bin/kicad-cli`
- KiCad bundled Python: `/Applications/KiCad/KiCad.app/Contents/Frameworks/Python.framework/Versions/3.9/bin/python3`

## Compatibility note

The existing Seeed Studio MCP server requires Python 3.10 or newer. KiCad's bundled `pcbnew` bindings are tied to Python 3.9. Text parsing and CLI validation can run without `pcbnew`; API-backed PCB editing requires a separately verified bridge or compatible server.
