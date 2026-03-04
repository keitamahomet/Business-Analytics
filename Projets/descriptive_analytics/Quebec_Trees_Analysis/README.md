# Quebec Trees Analysis

## Project Overview

This project analyzes a dataset of trees located in **Québec City**, using open data provided by the **Ville de Québec**.

The objective of the analysis is to identify **locations containing the largest number of trees** in order to help plan a potential outing for a group of tree enthusiasts (ADADQC – Amateurs d’Arbres de Québec).

In addition, the project computes several **descriptive statistics on tree characteristics**, particularly trunk diameter measurements, grouped by tree type.

This project was completed as part of the **MQT7021 – Business Analytics course** in the **MBA in Business Analytics program at Université Laval**.

---

# Dataset

The dataset comes from the **open data portal of the City of Québec** and contains detailed information about trees located throughout the city.

Each observation represents a **single tree**.

The dataset includes variables such as:
data/vdq-arbrerepertorie.csv

- Tree species (Latin and French names)
- Tree type (deciduous or conifer)
- Trunk diameter
- Measurement position
- Property type (public or private)
- Location (address)
- Geographic coordinates (latitude and longitude)

The data file used in this project is located in:

---

# Objectives

The main objectives of this analysis are:

1. Load the dataset using a **relative path**.
2. Verify whether any **parsing issues** occurred during data import.
3. Identify **missing values** across all variables.
4. Compute descriptive statistics on tree diameter.
5. Identify **public locations with the highest number of trees**.

---

# Methodology

The analysis was performed using **R** and the **tidyverse** packages.

The workflow includes the following steps:

### 1. Data Import

The dataset was loaded using the `read_csv()` function from the **readr** package.

The function `problems()` was used to verify whether any issues occurred during the import process.

---

### 2. Missing Value Analysis

The number of missing values was calculated for each column.

Special attention was given to the following variables, which should **not contain missing values**:

- ID
- LATITUDE
- LONGITUDE

---

### 3. Statistical Analysis

Descriptive statistics were calculated for trunk diameter measurements taken at **breast height (DHP)**.

The following statistics were computed:

- Mean diameter
- Standard deviation
- Minimum diameter
- Maximum diameter

These statistics were calculated:

- By **tree type**
- By **tree type and measurement position**

---

### 4. Identifying Potential Outing Locations

The analysis focused on **public properties only**.

Trees were counted by **topographical location (address)** in order to determine which locations contain the highest number of trees.

The **10 locations with the largest number of trees** were identified as potential outing destinations.

---

# Technologies Used

- R
- tidyverse
- dplyr
- readr
- ggplot2
- R Markdown

---

# Project Structure
Quebec_Trees_Analysis
│
├── README.md
├── trees_analysis.Rmd
├── trees_analysis.html
└── data
└── vdq-arbrerepertorie.csv

---

# Skills Demonstrated

- Data cleaning
- Data wrangling with tidyverse
- Missing data analysis
- Descriptive statistics
- Data aggregation and grouping
- Reproducible data analysis with R Markdown

---

# Author

Mahomet Limenia Jean-Yves J. Keita  
MBA – Supply Chain Management & Business Analytics  
Université Laval – Québec, Canada
