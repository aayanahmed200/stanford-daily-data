# Stanford Daily — Data Journalism Series

> A static index for four Stanford Daily data-journalism projects, linking each report and summarising the dataset and question behind it.

**Live series index:** [aayanahmed200.github.io/stanford-daily-data](https://aayanahmed200.github.io/stanford-daily-data/)

**Project reports:** [The Price of Prestige](https://aayanahmed200.github.io/stanford-daily-price-of-prestige/) · [PlasticList EDA](https://aayanahmed200.github.io/stanford-daily-plasticlist-eda/) · [Blotter Fiction](https://aayanahmed200.github.io/stanford-daily-blotter-fiction/) · [ICE Extraction Pipeline](https://aayanahmed200.github.io/stanford-daily-biglocal-ice-pipeline/)

[![HTML](https://img.shields.io/badge/html-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML) [![CSS](https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS) [![GitHub Actions](https://img.shields.io/badge/github%20actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/features/actions)

## Overview

This repository is the landing page and navigation index for a four-part Stanford Daily data-journalism series. It explains what each project investigates, identifies the underlying dataset or source material, and links readers to the published project page and source repository.

It is an index site, not the data-processing codebase for all four projects. Each project maintains its own analysis, scripts, and documentation in its respective repository.

## Projects in the series

- **The Price of Prestige** — College Scorecard and BLS data used to examine Stanford's published tuition, financial aid, student costs, and graduate outcomes.
- **PlasticList EDA** — exploratory analysis of 618 lab samples across 236 Bay Area food and beverage products, including Stanford dining samples.
- **Lot 95 — Blotter Fiction** — a fictional short story inspired by recurring patterns in 139 Stanford Daily police-blotter articles.
- **Big Local News ICE Extraction Pipeline** — a Python pipeline for extracting and validating structured information from public ICE press releases; the published coverage figures are based on a five-row smoke test.

## Implementation

The index is hand-written HTML and CSS with no framework or build step. A GitHub Actions workflow publishes the static contents of `site/` to GitHub Pages on pushes to `main`.

The shared series stylesheet is copied into this repository and the four project sites so the series masthead, footer, typography, and colour system remain consistent. When the shared design changes, the corresponding stylesheet copies need to be kept in sync.

## Repository structure

- `site/index.html` — series landing page.
- `site/series.css` — shared stylesheet used across the series sites.
- `site/favicon.png` — series site icon.
- `.github/workflows/pages.yml` — GitHub Pages publishing workflow.

## Run locally

Open `site/index.html` in a browser, or serve the `site/` directory with a local static server:

```bash
python -m http.server 8000 --directory site
```

## Status and limitations

The index is a static navigation and summary page. Its project descriptions and numerical summaries are taken from the individual repositories and are not recalculated here. The stylesheet is a copy shared with the project sites, so visual changes need to be synchronised across the repositories.

## License

MIT. See [LICENSE](LICENSE).
