# Golf Balance Device Research

Preliminary research and experiment design for a trial of the balance 
training device (proprietary design) applied to golf swing 
weight transfer.

## Background

The device was originally designed for ski training. It constrains the foot to 
medial edge loading via a rigid aluminium rail, mimicking the proprioceptive 
demand of ski edge engagement. Golf coaching literature identifies this same 
medial edge pressure pattern as critical to correct trail foot loading at the 
backswing transition.

No peer-reviewed trial of this device for golf exists. This project constitutes 
preliminary feasibility work.

## Repo Structure

```
golf-balance-research/
├── index.qmd                    # Site home
├── _quarto.yml                  # Quarto config
├── literature/
│   ├── evidence-register.qmd   # Systematic literature register
│   ├── extraction-prompt.md    # Reusable prompt for paper analysis
│   └── extractions/            # One .md file per extracted paper
├── experiment/
│   ├── design.qmd              # Trial protocol
│   ├── measures.qmd            # Outcome measures rationale
│   └── analysis-plan.qmd      # Pre-specified statistical approach
└── docs/                       # Quarto site output (GitHub Pages)
```

## Rendering the Site

```bash
quarto render
```

## GitHub Actions

This repository includes a GitHub Actions workflow at `.github/workflows/quarto-pages.yml`.
On every push to `main`, the workflow will:

- install Quarto
- render the site into `docs/`
- deploy the generated site to the `gh-pages` branch

## GitHub Pages setup

After you push this repository to GitHub, enable Pages from:

1. `Settings` → `Pages`
2. `Source` → `gh-pages` branch
3. `Folder` → `/ (root)`

If your branch is not `main`, update the workflow branch name accordingly.

## Status

- [x] Repo structure
- [ ] Literature review — in progress
- [ ] Experiment design — draft complete, awaiting literature review input
- [ ] Ethics consideration
- [ ] Data collection

## Collaborators

- Golf instructor (expert consultant)
- Device inventor (to be confirmed)
- Data analysis: T. Simm
