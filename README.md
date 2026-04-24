# Blank Card Paradox

An interactive research website exploring how blank wildcard cards changed puzzle-solving behavior in a cognitive psychology study.

## Overview

This repository contains a static GitHub Pages site for the **Blank Card Paradox** project. The site presents the study as a visual data story, combining a landing page, a research narrative, and an interactive participant viewer built from the LMU analysis dataset.

## What The Site Includes

- `index.html` — a landing page introducing the puzzle, the paradox, and the main findings
- `research.html` — a narrative walkthrough of the experiment with charts and participant summaries
- `viewer.html` — an interactive viewer for recorded participant move sequences and final board layouts
- `data.js` — a local browser-ready dataset generated from the LMU CSV export

## Key Findings

- `229` participants across four experimental conditions
- `60` participants used blank cards
- `73.3%` success rate for participants who used blank cards
- `37.3%` success rate for participants who did not use blank cards
- Strongest blank-card effect in `KQB`, where blanks were both more visible and more useful

## Data Source

The site is powered by a local generated dataset:

- Source CSV: `Data for LMU analyses 13 aug 2025.csv`
- Generated asset: `data.js`

The website does not need a backend or database. Once `data.js` is present, the project can be deployed as a plain static site.

## Regenerate The Dataset

Run:

```bash
python3 src/build_cardiee_data.py '/Users/shana/Downloads/Data for LMU analyses 13 aug 2025.csv' '/Users/shana/msc project/outputs/figures/cardiee/files/data.js'
```

## Publish On GitHub Pages

1. Push this folder to the root of a GitHub repository.
2. Open the repository on GitHub.
3. Go to `Settings` -> `Pages`.
4. Choose `Deploy from a branch`.
5. Select branch `main` and folder `/ (root)`.

GitHub Pages will serve `index.html` automatically.

## Notes

- This is a static site with no backend dependencies.
- The participant data is already bundled locally in `data.js`.
- Google Fonts and Chart.js are still loaded from CDNs.

## Suggested Repository Description

Interactive research website for the Blank Card Paradox study, visualizing puzzle-solving behavior, blank-card usage, and participant move data.
