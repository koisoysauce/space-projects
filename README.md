# Space Data Projects

A progressive series of Python data science projects exploring real NASA and ESA datasets. These projects cover planetary science, asteroid classification, and exoplanet analysis.

## Goal

To develop the data science and computational skills needed for space research and analysis, with each project building toward a Gaia DR3 stellar classification project.

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

Projects 02–05 will be added as they are completed.

## How This Repo is Organized

Each project lives in its own numbered folder with a consistent structure:

```
XX-project-name/
├── data/           # raw downloaded datasets (not tracked in git if large)
├── notebook.ipynb  # main Jupyter notebook
└── README.md       # what the project is, what I did, what I found
```
