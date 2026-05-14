# Exercise #06 - Data Analysis Report

This repository contains the resolution for Exercise #06 using the `EFIplus_medit` dataset.

## 📊 Visual Analysis & Transformations
* **Points 1 & 2:** Variables like `Altitude` and `Actual_river_slope` showed high positive skewness. I applied a $log_{10}(x+1)$ transformation to normalize the data for parametric tests.
* **Plots:** See `distributions_before.png` and `distributions_after.png`.

## 🧬 Species Richness
* **Point 3:** Created a `richness` column by summing all species presence/absence columns (starting from *Abramis brama*).
* **Data:** The final values are available in `Exercise_06_Final_Results.csv`.

## 📍 Outlier Detection
* **Point 4:** Performed a bivariate outlier detection between Mean Annual Temperature and Species Richness using an **Isolation Forest** model (5% contamination).
* **Plot:** See `outliers.png`.

## 🌍 Regional Comparison
* **Point 5:** Explored the relationship across different countries. The results suggest that the influence of temperature on richness varies geographically.
* **Plot:** See `countries.png`.
