# Publication change log

## 2026-10-27 — First documented GitHub-ready portfolio package

- Added a professional project README, business case, data dictionary, workflow, limitations and attribution.
- Preserved the supplied original NYC inspection CSV and LA OSM-derived CSV in `data/raw/`.
- Preserved both author's final submitted Excel files **unchanged** in `data/submitted_workbooks/`.
- Created clean UTF-8 with BOM city-specific and combined five-column CSV export files.
- Created a separate portfolio workbook and quality-assurance report.
- Cleared **five** visibly third-party or expressly unofficial website URLs *only in the publication copies*. Exact changes and evidence are logged in `quality_assurance/publication_adjustments.csv`.
- Did not delete restaurant records, fabricate contacts, change addresses, or overwrite the original submitted workbooks.
- Identified issues that still need manual validation; no blanket claim of current contact verification or exhaustive city coverage.

The original data-preparation and manual web-research work were performed by the portfolio author. This package is a presentation and transparent structural-audit handoff; it does not pretend to reconstruct unprovided Power Query steps or source-by-source verification dates.
