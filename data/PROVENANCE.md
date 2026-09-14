# Data provenance - supplement site

Every file here is **aggregate-only** and safe to publish, produced by
`working_code/analysis/export_site_data.R` from the research repo's
already-aggregated `paper/tables/*.csv`.

## Confidentiality rule (enforced at export)

- Allowlist only: full-sample / arm / intensity / asset-category aggregates.
- Export refuses any file carrying a bank/LEI/entity identifier column.
- No per-bank or per-country rows, so no cell resolves to < 3 banks.
- Country- and bank-level tables are intentionally NOT exported here.

## Files

| file | source | rows | cols |
|------|--------|------|------|
| `mask_summary_eba.csv` | `tab_mask_summary.csv` | 40 | 37 |
| `mask_summary_giips_debt.csv` | `tab_mask_summary_giips_debt.csv` | 28 | 37 |
| `mask_summary_russia_shock.csv` | `tab_mask_summary_russia_shock.csv` | 28 | 37 |
| `mask_summary_asian_debt.csv` | `tab_mask_summary_asian_debt.csv` | 28 | 37 |
| `mask_summary_north_res.csv` | `tab_mask_summary_north_res.csv` | 28 | 37 |
| `mask_summary_south_res.csv` | `tab_mask_summary_south_res.csv` | 28 | 37 |
| `contagion_summary_eba.csv` | `tab_contagion_summary.csv` | 52 | 12 |
| `contagion_summary_giips_debt.csv` | `tab_contagion_summary_giips_debt.csv` | 40 | 7 |
| `contagion_summary_russia_shock.csv` | `tab_contagion_summary_russia_shock.csv` | 20 | 7 |
| `contagion_summary_asian_debt.csv` | `tab_contagion_summary_asian_debt.csv` | 20 | 7 |
| `contagion_summary_north_res.csv` | `tab_contagion_summary_north_res.csv` | 20 | 7 |
| `contagion_summary_south_res.csv` | `tab_contagion_summary_south_res.csv` | 20 | 7 |
| `shapley_decomp.csv` | `tab_shapley_decomp.csv` | 4 | 24 |
| `sensitivity_freeze.csv` | `tab_sensitivity_freeze.csv` | 19 | 12 |
| `sensitivity_fsa.csv` | `tab_sensitivity_fsa.csv` | 5 | 11 |
| `sensitivity_rho.csv` | `tab_sensitivity_rho.csv` | 5 | 11 |
| `sensitivity_run_k1.csv` | `tab_sensitivity_run_k1.csv` | 5 | 11 |
| `convergence.csv` | `tab_convergence.csv` | 40 | 3 |
| `distress_streak.csv` | `tab_distress_streak_summary.csv` | 1 | 7 |
| `collateral_pool.csv` | `tab_validation_collateral_pool.csv` | 5 | 3 |
| `calibration_friction.csv` | `tab_calibration_friction.csv` | 14 | 3 |
