# Space Data Projects

A progressive series of Python data science projects working toward Gaia DR3 stellar classification. Built as a self-study portfolio over Summer 2026, each project builds on the skills of the last.

## Goal

To develop the data science and computational skills for space research and analysis.

## Stack

- **Python** — pandas, numpy, matplotlib, seaborn, scipy
- **Machine Learning** — scikit-learn
- **Astronomy** — astropy, astroquery (introduced in later projects)
- **Environment** — Jupyter notebooks

## Project Progression

| # | Project | Skills Introduced | Dataset |
|---|---------|-------------------|---------|
| 01 | [Planet Analysis](./01-planet-analysis/) | pandas basics, EDA, matplotlib, feature engineering | NASA Planetary Fact Sheet |
| 02 | Asteroid Explorer | Data cleaning, `.groupby()`, `.merge()`, correlation heatmaps | NASA Asteroids — Kaggle |
| 03 | Exoplanet Explorer | Multi-variable scatter plots, colormaps, log scaling | NASA Exoplanet Archive |
| 04 | Hipparcos H-R Diagram | FITS-adjacent data, absolute magnitude, parallax | Hipparcos Catalog |
| 05 | Asteroid Hazard Classification | scikit-learn pipeline, Random Forest, confusion matrix | NASA Nearest Earth Objects |
| 06 | Gaia Stellar Classification | astroquery, Gaia DR3, full ML classification pipeline | Gaia DR3 |

Projects 02–06 will be added as they are completed.

## How This Repo is Organized

Each project lives in its own numbered folder with a consistent structure:

```
XX-project-name/
├── data/           # raw downloaded datasets (not tracked in git if large)
├── notebook.ipynb  # main Jupyter notebook
└── README.md       # what the project is, what I did, what I found
```
