# Stanford Daily: Data series

**Live:** [aayanahmed200.github.io/stanford-daily-data](https://aayanahmed200.github.io/stanford-daily-data/)

**Series:** [The Price of Prestige](https://aayanahmed200.github.io/stanford-daily-price-of-prestige/) · [PlasticList](https://aayanahmed200.github.io/stanford-daily-plasticlist-eda/) · [Blotter fiction](https://aayanahmed200.github.io/stanford-daily-blotter-fiction/) · [ICE pipeline](https://aayanahmed200.github.io/stanford-daily-biglocal-ice-pipeline/)

[![HTML](https://img.shields.io/badge/html-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML) [![GitHub Actions](https://img.shields.io/badge/github%20actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/features/actions)

The index for four Stanford Daily data projects: what each one is, what data it uses, and why it exists.

## Overview

Each project takes one public dataset and reports what it says. This page is the entry point: it lists the four reports, summarises the question behind each, and links to the full page and the code.

## How it was made

Hand-written HTML and CSS with no framework and no build step: one page, one stylesheet and one icon, published straight from `site/` by a GitHub Actions workflow on every push to `main`.

The stylesheet is the same file the four project pages serve, copied byte for byte, so the series header, footer, type scale and colours come from one source. Each project page links back here and to its three siblings, and this page links out to all four.

## Highlights

- **The Price of Prestige** — College Scorecard: sticker price versus net price, the aid curve, a 25-year tuition trend, earnings ten years out, and a regression over 530 colleges that separates the school's effect from the family income of the students it admits.
- **Plastic in the Pantry** — PlasticList: 618 lab samples across 236 Bay Area food and beverage products, including a Stanford dining-hall meal.
- **Lot 95** — a short story built from 139 Stanford Daily police-blotter articles published between 2021 and 2026.
- **Reading 965 ICE press releases as data** — a pipeline that extracts dateline locations, people, agencies, money and action categories from the Big Local News ICE dataset, with a validation report.

## Repository contents

- `site/index.html` — the series index page.
- `site/series.css` — the shared stylesheet, identical to the copy each project site serves.
- `site/favicon.png` — the site icon, shared with the four projects.
- `.github/workflows/pages.yml` — publishes `site/` to GitHub Pages on every push to `main`.

## Notes and limitations

The summaries describe the datasets and methods stated in each project's repository. Numbers are quoted from those projects, not recomputed here. The page is static HTML with no build step, so editing `site/index.html` is the whole workflow. `site/series.css` is a copy: a change is made in one project site, then copied to the other four repositories so all five stay identical.

## License

MIT
