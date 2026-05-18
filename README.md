# Golf Balance Research

Preliminary research and experiment design for a study of balance-focused 
training applied to golf swing weight transfer.

## Background

This project explores whether targeted balance and foot-pressure training can 
produce measurable changes in centre of pressure timing, weight transfer, and 
ball-striking outcomes during the golf swing.

This project constitutes preliminary feasibility work before any formal data 
collection.

## Repo Structure

```
golf-balance-research/
├── index.qmd                    # Site home
├── _quarto.yml                  # Quarto config
├── literature/
│   ├── evidence-register.qmd   # Systematic literature register
│   ├── extraction-prompt.md    # Reusable prompt for paper analysis
│   └── extractions/            # One .md file per extracted paper
├── experiment/                 # Local-only working files, ignored by git
│   ├── design.qmd              # Trial protocol
│   ├── measures.qmd            # Outcome measures rationale
│   └── analysis-plan.qmd      # Pre-specified statistical approach
└── _site/                      # Local Quarto render output, ignored by git
```

## Rendering the Site

```bash
quarto render
```

## GitHub Actions

This repository includes a GitHub Actions workflow at `.github/workflows/quarto-pages.yml`.
On every push to `main`, the workflow will:

- install Quarto
- render the site into `_site/`
- deploy the generated site with GitHub Pages

## GitHub Pages setup

After you push this repository to GitHub, enable Pages from:

1. `Settings` → `Pages`
2. `Source` → `GitHub Actions`

If your branch is not `main`, update the workflow branch name accordingly.

## Status

- [x] Repo structure
- [ ] Literature review — in progress
- [ ] Experiment design — draft complete, awaiting literature review input
- [ ] Ethics consideration
- [ ] Data collection

## Collaborators

- Golf instructor (expert consultant)
- Data analysis: T. Simm
