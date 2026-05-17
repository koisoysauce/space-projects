# 01 — Planet Analysis

**Skills practiced:** pandas DataFrame creation, EDA, feature engineering, matplotlib visualizations, physical law verification

## The Dataset

NASA Planetary Fact Sheet data for all 8 planets, manually constructed as a pandas DataFrame. Includes mass, diameter, surface gravity, number of moons, orbital period, distance from the Sun, and mean temperature.

Source: https://www.kaggle.com/datasets/joebeachcapital/planets-and-moons?resource=download

## What I Did

**Data exploration**
loaded the dataset and ran standard EDA: `.shape`, `.dtypes`, `.describe()`, and null checks to understand the structure before doing anything else.

**Feature Engineering**
1. Added M/r² column to the dataset for easier plotting
2. Added orbital period in earth years column to compare planets year lengths in comparison to earth
3. Added my weight column to compare my weight between planets

**Visualizations**
1. Plot of moon count vs. planet diameter to infer relation between moon count and planet size
2. Graph of M/r² (kg/m²) vs. Acceleration of Gravity to confirm Newton's Law of Universal Gravitation: M/r² ∝ g
3. Bar chart of orbital period relative to Earth to compare year lengths between planets
4. Graph of T² (orbital period) vs. R³ (distance from Sun) to confirm Kepler's Third Law: T² ∝ R³
5. Graph of gravity (m/s²) vs. weight (N) to confirm Newton's Second Law: W ∝ g

## What I Found

- There appears to be a relation between the number of moons orbiting a planet and the size of the planet, but there is no evidence from this plot due to the small sample size of only 9 planets.
- A nearly fully linear graph is seen from the M/r² vs. g graph, with the slope giving a 7.01% error from G, the gravitational constant, confirming Newton's Law of Universal Gravitation.
- Saturn slightly veers off from the trend in the M/r² vs. g graph, likely due to rounding since Saturn is the least dense planet in the dataset, making it sensitive to slight measurement errors in mass and/or diameter.
- The bar chart of orbital period relative to Earth shows that as a planet is further from our Sun, the orbital period in Earth years increases, which plays into Kepler's Third Law.
- The T² vs. R³ graph confirms Kepler's Third Law, showing a linear graph with a correlation coefficient of 1.0.
- gravity vs. weight graph shows a correlation coefficient of 1.00 and a slope of 55.0, giving a percent error of 0.00%, confirming Newton's Second Law.