# Projects

This folder contains projects developed during my **MBA in Business Analytics at Université Laval**.  
The projects cover **descriptive, predictive, and prescriptive analytics**, using real-world datasets and analytical methods to support data-driven decision making.

---

# Descriptive Analytics and Data Analysis in R

📅 Sept. 2025 – Dec. 2025  
🎓 Université Laval – MBA Business Analytics (MQT7021)

Several data analysis projects were developed in **R** using real datasets from governmental and organizational sources.

## Tree Data Analysis – Québec

Descriptive analysis of a public dataset containing information about trees in Québec.

**Tasks performed**

- Data cleaning and preprocessing
- Missing value analysis
- Descriptive statistics (mean, standard deviation, min, max)
- Analysis by tree type and measurement position

**Objective**

Identify structural trends and public locations with the highest number of trees.

**Tools**

R, tidyverse, dplyr, readr, ggplot2

---

## Retail Traffic Analysis – "Chez Tony"

Analysis of hourly customer traffic data for a retail business.

**Tasks performed**

- Data transformation to **tidy format**
- Temporal analysis by:
  - hour
  - day
  - week
- Visualization of peak traffic periods

**Objective**

Identify peak demand periods to support **operational decision-making**.

**Tools**

R, tidyverse, lubridate, ggplot2

---

## Weather Impact on Employee Activity

Analysis combining:

- weather data from **Environment Canada**
- employee login data

**Tasks performed**

- Data cleaning and missing value handling
- Feature engineering
  - good weather
  - critical period
  - weekend
- Dataset merging and comparative analysis

**Objective**

Evaluate the impact of **weather conditions and external measures on employee activity**.

**Tools**

R, tidyverse, ggplot2

---

# Prescriptive Analytics and Mathematical Programming

📅 Sept. 2025 – Dec. 2025  
🎓 Université Laval

Development of **optimization models in R** using the package **CVXR** and other optimization approaches.

## Multi-period Investment Portfolio Optimization

Optimization model maximizing investment returns over **8 years**.

**Initial budget**

550,000 $

**Constraints**

- liquidity constraints
- no borrowing
- reinvestment dynamics

**Result**

Optimal investment strategy reaching **612,612 $**.

**Tools**

R, CVXR, GLPK

---

## Production–Sales–Inventory Optimization

Optimization model maximizing net profit across **4 periods**.

**Constraints**

- production capacity
- minimum contractual sales
- storage costs

**Result**

Optimal production and inventory strategy reaching **3,386 $ profit**.

---

## Combinatorial Optimization – Minimum Coverage

Problem of minimizing the number of cameras needed to cover all strategic locations in a building.

Approaches tested:

- Integer programming (exact solution)
- Random search
- Genetic algorithm

**Tools**

R, GLPK

---

# Predictive Analytics – Machine Learning in R

📅 Sept. 2025 – Dec. 2025  
🎓 Université Laval

Projects applying **machine learning algorithms to real datasets**.

---

## Sales Analysis and Weather Impact – Willmart

Analysis of sales performance based on weather conditions.

**Data preparation**

- cleaning and transformation
- merging sales and weather datasets

**Methods**

- exploratory analysis
- K-means clustering
- elbow method for optimal clusters

**Objective**

Identify sales behavior patterns based on climate conditions.

---

## Greenhouse Gas Emission Prediction

Supervised regression model predicting annual greenhouse gas emissions of Québec companies.

**Models tested**

- KNN
- Neural Network
- Random Forest

**Evaluation metrics**

- RMSE
- MAE
- R²

**Best model**

KNN provided the best balance between accuracy and robustness.

---

# Data Engineering and Database Design

Design of a **relational database** from raw CSV datasets.

**Tools**

R (tidyverse), DBI, RSQLite

**Steps**

- Data cleaning and validation
- Primary and foreign key verification
- Removal of duplicates and inconsistencies
- Database normalization

**Database structure**

- companies
- categories
- locations
- types

**Analytical SQL queries**

- company filtering by period
- geographic analysis
- median founding year calculation
- company aggregation by category
