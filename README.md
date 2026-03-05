
# Energy Market Intelligence & ML: Global Renewable Transition Case Study

### UN Energy Statistics Portfolio (2019–2023)

**Author:** Diana Nicuțari


---

## 📋 Project Overview

This repository provides a sophisticated end-to-end analysis of the global shift toward wind and solar energy, utilizing the **UN Energy Statistics Database**. The project moves beyond descriptive statistics to deliver actionable market intelligence through machine learning and robust statistical forecasting.

---

## 🛠️ Technical Stack

* **Data Wrangling:** `pandas` & `numpy` for multi-million row manipulation and merging.
* **Machine Learning:** `scikit-learn` (K-Means Clustering) for global market segmentation.
* **Forecasting:** `statsmodels` (Holt-Winters Exponential Smoothing) for time-series projections.
* **Visualization:** `seaborn` & `matplotlib` for publication-quality analytics.

---

## 🗂️ Data Strategy & ETL

To bypass the 100,000-row limit of the UN Statistics Database, the project utilizes a targeted extraction strategy focusing on four key commodity slices: **Total Wind**, **Total Solar**, **Gross Production**, and **Final Consumption**.

* **Reporting Lag Mitigation:** The analysis window is strictly locked to **2019–2023** to ensure an "apples-to-apples" comparison and eliminate administrative noise from incomplete 2024 filings.
* **Baseline Filtering:** Implemented a **100 million kWh production threshold** to eliminate statistical "noise" from micro-grids and focus on meaningful infrastructure.

---

## 🔬 Analysis Methodology

### 1. Identifying "Aggressive Adopters" (Growth Velocity)

The analysis distinguishes between absolute volume and **adoption velocity**. By calculating the 5-year average annual growth rate, this study identifies "frontier markets" that are leapfrogging traditional fossil fuel infrastructure.

### 2. Market Segmentation (K-Means Clustering)

The world is grouped into four distinct "energy tribes" using unsupervised machine learning.

* **Feature Engineering:** Mapping Renewable % against Total Grid Size.
* **Normalization:** Applied a **logarithmic scale** (`Log1p`) to total grid sizes to allow for balanced comparisons between global superpowers and emerging markets on a single visualization.

### 3. Forecasting the UK’s 2030 Horizon

Projected the UK's wind energy output using **Holt-Winters Exponential Smoothing**.

* **Model Configuration:** Selected an **Additive Trend** model to account for the compounding nature of the UK's wind infrastructure growth rather than a simple linear regression.

---

## 📈 Strategic Insights

* **The "Sprinter" vs. "Giant" Paradox:** The project identifies that while the USA and China lead in absolute volume, frontier markets often demonstrate a higher relative "momentum" in grid transition.
* **2030 Outlook:** Data-backed projections for the UK indicate a sustained compounding growth trajectory, providing a baseline for grid modernization planning.

---
