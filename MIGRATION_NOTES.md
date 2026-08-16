# Migration Baseline — StockgroupSummary (Pilot Client)

- Migration date: 2026-08-16
- Source (pre-migration): `C:\Arti\D\Claude work space\StockgroupSummary`
- Migrated by: Claude Desktop (Phase 1 of TDL → GitHub → Claude Desktop Transformation Roadmap)
- Status: Baseline commit only. Contents preserved exactly as found; no refactoring performed.

## Files in this baseline
- `main.txt` — entry point, includes `Stockgroupwise Report.txt`
- `Stockgroupwise Report.txt` — active TDL source (Stock Groupwise/Partywise report)
- `Stockitemwise Report.txt` — TDL source, currently commented out of `main.txt` (not included at runtime)
- `StockgroupSummary.tpj` — Tally Developer project file
- `StockgroupSummary.tcp` — compiled Tally Compiled Package (binary build output, not source)
- `WhatsApp Image 2023-08-31 at 22.58.26.jpeg` — supporting image (purpose not yet documented)

## Notes for Phase 2 (structure standardization)
- Consider whether `StockgroupSummary.tcp` (compiled binary) should be gitignored going forward and rebuilt from source instead of tracked.
- `Stockitemwise Report.txt` is present but not currently wired into `main.txt` — confirm whether it's legacy/inactive before documenting it as ACTIVE in the module knowledge base (Phase 3).
- A duplicate archive (`StockgroupSummary.zip`) exists at the workspace root — treat as a historical snapshot, not a second source of truth.

## Secret scan
Scanned all text files for API keys, passwords, tokens. None found. (Note: unrelated files elsewhere in the workspace, e.g. `Imp Code/Pwd lock vch new.txt`, contain literal "pwd" in the name and should be reviewed before any future client folder is migrated.)
