# Data provenance - supplement site

Every file here is **aggregate-only** and safe to publish, produced by
`working_code/analysis/export_site_data.R` from the research repo's
already-aggregated `paper/tables/*.csv` (and, for the phase-space
trajectories, from group-aggregated headline liabilities).

## Confidentiality rule (enforced at export)

- Allowlist only: full-sample / arm / intensity / asset-category aggregates,
  plus country-group trajectories pooled to >= 3 banks.
- Export refuses any file carrying a bank/LEI/entity identifier column.
- No cell resolves to < 3 banks.
- Country- and bank-level source tables are intentionally NOT exported.

## Files

| file | source | rows | cols |
|------|--------|------|------|
| `shapley_decomp.csv` | `tab_shapley_decomp.csv` | 4 | 24 |
| `sensitivity_freeze.csv` | `tab_sensitivity_freeze.csv` | 19 | 12 |
| `sensitivity_fsa.csv` | `tab_sensitivity_fsa.csv` | 5 | 11 |
| `sensitivity_rho.csv` | `tab_sensitivity_rho.csv` | 5 | 11 |
| `sensitivity_run_k1.csv` | `tab_sensitivity_run_k1.csv` | 5 | 11 |
| `sensitivity_freeze_i1.csv` | `tab_sensitivity_freeze_i1.csv` | 19 | 12 |
| `sensitivity_fsa_i1.csv` | `tab_sensitivity_fsa_i1.csv` | 5 | 11 |
| `sensitivity_rho_i1.csv` | `tab_sensitivity_rho_i1.csv` | 5 | 11 |
| `sensitivity_run_k1_i1.csv` | `tab_sensitivity_run_k1_i1.csv` | 5 | 11 |
| `convergence.csv` | `tab_convergence.csv` | 40 | 3 |
| `distress_streak.csv` | `tab_distress_streak_summary.csv` | 1 | 7 |
| `collateral_pool.csv` | `tab_validation_collateral_pool.csv` | 5 | 3 |
| `calibration_friction.csv` | `tab_calibration_friction.csv` | 14 | 3 |
| `phase_space.csv` | `headline/eba liabilities (group-aggregated)` | 2665 | 7 |
| `mask_summary_eba.csv` | `tab_mask_summary.csv (I<=1.00, normalised)` | 40 | 38 |
| `contagion_summary_eba.csv` | `tab_contagion_summary.csv (I<=1.00, normalised)` | 52 | 13 |
| `mask_summary_giips_debt.csv` | `tab_mask_summary_giips_debt.csv (I<=1.00, normalised)` | 28 | 38 |
| `contagion_summary_giips_debt.csv` | `tab_contagion_summary_giips_debt.csv (I<=1.00, normalised)` | 40 | 8 |
| `mask_summary_russia_shock.csv` | `tab_mask_summary_russia_shock.csv (I<=1.00, normalised)` | 28 | 38 |
| `contagion_summary_russia_shock.csv` | `tab_contagion_summary_russia_shock.csv (I<=1.00, normalised)` | 20 | 8 |
| `mask_summary_asian_debt.csv` | `tab_mask_summary_asian_debt.csv (I<=1.00, normalised)` | 28 | 38 |
| `contagion_summary_asian_debt.csv` | `tab_contagion_summary_asian_debt.csv (I<=1.00, normalised)` | 20 | 8 |
| `mask_summary_north_res.csv` | `tab_mask_summary_north_res.csv (I<=0.20, normalised)` | 20 | 38 |
| `contagion_summary_north_res.csv` | `tab_contagion_summary_north_res.csv (I<=0.20, normalised)` | 20 | 8 |
| `mask_summary_south_res.csv` | `tab_mask_summary_south_res.csv (I<=0.20, normalised)` | 20 | 38 |
| `contagion_summary_south_res.csv` | `tab_contagion_summary_south_res.csv (I<=0.20, normalised)` | 20 | 8 |
| `channel_liquidity.csv` | `input/{haircuts,repo_haircuts,max_discounts}.csv (schedule)` | 21 | 3 |
