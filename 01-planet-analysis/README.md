# 01 — Planet Explorer

**Skills practiced:** pandas DataFrame creation, EDA, feature engineering, matplotlib charts and plots

## The Dataset

NASA Planetary Fact Sheet data for all 8 planets, manually constructed as a pandas DataFrame. Includes mass, diameter, surface gravity, number of moons, orbital period, distance from the Sun, and mean temperature.

Source: https://www.kaggle.com/datasets/joebeachcapital/planets-and-moons?resource=download

## What I Did

**Data exploration** — loaded the dataset and ran standard EDA: `.shape`, `.dtypes`, `.describe()`, and null checks to understand the structure before doing anything else.

**Feature Engineering** —

**Visualizations** — built plots:
1. Plot of moon count vs. planet diameter to infer relation between the two

## What I Found

- There appears to be a relation between the number of moons orbiting a planet and the size of the planet, but there is no evidence from this plot due to the small sample size of 9 planets, all the planets orbiting our solar system.

## Key Pandas/Numpy Skills Used

```python
pd.DataFrame()             # constructing a DataFrame from scratch
df.describe()              # summary statistics
df.isnull().sum()          # null checking
df['new_col'] = ...        # feature engineering
```