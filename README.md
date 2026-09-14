# CBCF Stress Test - Navigator

Interactive companion to the working paper *Collateral Constraints and Endogenous
Liquidity Stress: The Central Bank Collateral Framework as a Financial Stability
Tool* (Cuzzola, Barbieri & Bindseil).

This is a **static Quarto website**, published to GitHub Pages by the workflow in
`.github/workflows/publish.yml` on every push to `main`.

## Confidentiality

This repository is public and contains **no confidential data**. Everything under
`data/` is aggregated to groups of at least three banks and is produced by an export
step in the (private) research repo. The supervisory inputs and the decryption key
never enter this repo; `.gitignore` blocks them as a backstop. See
`data/PROVENANCE.md`.

## Build locally

```bash
quarto preview      # live preview at localhost
quarto render       # build static site into _site/
```

## Structure

- `index.qmd` — home
- `pages/` — model, results, scenario explorer, robustness, methods
- `data/` — aggregate, non-confidential exports (committed)
- `assets/` — static images and JS/SVG for the conceptual visuals

## Status

Scaffold (milestone M0). Content is added incrementally per the build plan in the
research repo, `docs/plans/2026-09-14_supplemental-website.md`.
