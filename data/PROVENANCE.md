# Data provenance — supplement site

Every file in this directory is **aggregate-only** and safe to publish. It is
produced by an explicit export step from the research repo's already-aggregated
`paper/tables/*.csv` (see `docs/plans/2026-09-14_supplemental-website.md`, §5).

## Confidentiality rule (enforced before every publish)

- Every statistic resolves to **at least three banks**. Country / business-model
  groups below the floor are pooled into a residual group.
- No `bank_id`, no per-bank rows, no sub-3-bank cells.
- This repo never contains the supervisory inputs (`input/banks/`,
  `business_models.csv`) or the decryption key; `.gitignore` blocks them.

## Files

_(none yet — populated at milestone M1 by `export_site_data.R`)_

| file | source script | contents | aggregation |
|------|---------------|----------|-------------|
| — | — | — | — |
