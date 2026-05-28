# Better Life Index: Statistical Analysis of Life Satisfaction 📊✨

## 📌 Project Overview
This project focuses on a comprehensive statistical analysis and modeling of the factors influencing subjective "happiness" or life satisfaction across different countries. 

Using cross-national data, the study aims to identify which socio-economic aspects (such as income, employment, safety, and environmental quality) act as key drivers of `Life satisfaction`[cite: 1]. Additionally, it segments countries into homogenous clusters based on their overall quality-of-life indicators[cite: 1].

## 🗃️ Dataset Description
The empirical foundation of this study is the **OECD Better Life Index (2024)** dataset[cite: 1].
* **Data Volume:** 40+ country observations[cite: 1].
* **Features:** 26 quantitative indicators reflecting multi-dimensional well-being (e.g., GDP per capita, employment rate, housing expenditure, water quality, life expectancy, crime rates, etc.)[cite: 1].

## 🎯 Project Goals & Tasks
**Main Objective:** Conduct a multi-dimensional statistical analysis of global life satisfaction using cross-sectional country-level data.

**Key Tasks:**
1. **Exploratory Data Analysis (EDA):** Analyze the structure, descriptive statistics, and distribution of the target variable `Life satisfaction`.
2. **Data Visualization:** Identify ranges, density distributions, and potential outliers using visualization tools (Dotplots, Boxplots, etc.).
3. **Clustering:** Segment countries into uniform groups based on their comprehensive well-being profiles.
4. **Regression Analysis:** Build and evaluate econometric models for each specific cluster to uncover localized drivers of life satisfaction.

## 🛠️ Tech Stack
* **Data Manipulation & Math:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning & Econometrics:** `scikit-learn` (Clustering), `statsmodels` (Linear Regression)

## 📈 Key Findings & Insights
By clustering the countries and applying separate regression models to each group, the following patterns emerged:

* 🟢 **Cluster 0 (Moderate Fit, $R^2 = 0.53$):** Roughly half of the variance in life satisfaction is explained by the model's features. **GDP per capita** (income) is the dominant and statistically significant driver[cite: 1]. Interestingly, traditional factors like employment rate and life expectancy were found to be statistically insignificant (high $p$-values) within this cluster[cite: 1].
* 🟡 **Cluster 1 (Weak Fit, $R^2 = 0.20$):** Traditional economic and social factors yield high $p$-values and fail to explain variations in life satisfaction[cite: 1]. This is highly characteristic of highly developed nations where basic material needs are fully met, meaning happiness begins to depend on more nuanced social, cultural, or individual psychological factors[cite: 1].
* 🔵 **Cluster 2 (Strong Fit, $R^2 = 0.81$):** The chosen features explain the vast majority of the variance. **GDP per capita** remains the single strongest positive driver[cite: 1]. While the small sample size within this cluster requires caution when interpreting exact $p$-values, the overall macroeconomic trend is exceptionally strong[cite: 1].
