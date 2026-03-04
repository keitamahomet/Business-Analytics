# Predictive Analytics Projects

## Overview

This repository presents two predictive analytics projects developed as part of a graduate-level course in Business Analytics. The objective of these projects is to explore how data science and machine learning techniques can be used to extract insights and build predictive models to support decision-making.

The analyses were conducted using the R programming language and focus on two different real-world inspired datasets: retail sales influenced by weather conditions and greenhouse gas emissions produced by companies. These projects illustrate the complete data analytics workflow including data cleaning, exploratory data analysis, feature preparation, model training, evaluation, and interpretation of results.

---

## Project 1 – Weather and Sales Analysis

### Objective

The first project investigates the relationship between weather conditions and retail sales performance. The goal is to determine whether temperature and precipitation influence product sales and to identify patterns in the data that could help managers better understand demand variations.

### Methodology

The analysis begins with data preprocessing and cleaning to ensure consistency and reliability. This includes handling missing values, filtering relevant observations, and converting measurements from imperial units to metric units.

Exploratory data analysis is then performed using visualizations to understand the distribution of sales across products and time periods. The best-selling product is identified and further analyzed to examine how weather conditions affect its daily sales.

To uncover hidden structures in the data, clustering techniques are applied using the k-means algorithm. Sales, temperature, and precipitation variables are used to group observations and identify possible segments where weather conditions influence purchasing behavior.

### Key Techniques

* Data cleaning and transformation
* Exploratory data analysis
* Data visualization with ggplot2
* K-means clustering
* Elbow method for cluster selection

### Tools Used

* R
* tidyverse
* ggplot2
* stats (kmeans)

---

## Project 2 – Greenhouse Gas Emissions Prediction

### Objective

The second project focuses on predicting the average annual greenhouse gas emissions of companies based on their characteristics and geographic location. The objective is to determine whether machine learning models can accurately estimate emissions for new companies.

### Problem Type

This problem is formulated as a **regression task** since the target variable represents a continuous numeric value corresponding to average yearly emissions.

### Data Preparation

The dataset includes information such as company category, longitude, and latitude. Non-informative attributes such as company names and industry codes are removed before model training. The dataset is separated into training and testing subsets to ensure proper evaluation.

### Machine Learning Models

Several predictive models are trained and evaluated using the **caret** framework in R.

The models include:

* K-Nearest Neighbors (KNN)
* Neural Networks
* Random Forest

Hyperparameter tuning and cross-validation are used to optimize model performance. The models are evaluated on the test dataset using metrics such as Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R-squared.

### Results

Among the tested models, the **K-Nearest Neighbors model achieved the best predictive performance**, producing the lowest error metrics on the test dataset.

### Key Techniques

* Data preprocessing
* Feature selection
* Cross-validation
* Hyperparameter tuning
* Model evaluation

### Tools Used

* R
* tidyverse
* caret
* machine learning algorithms

---

## Key Skills Demonstrated

These projects demonstrate several important skills in data analytics and machine learning:

* Data cleaning and preprocessing
* Exploratory data analysis (EDA)
* Statistical analysis
* Data visualization
* Machine learning model development
* Model evaluation and comparison
* Feature engineering

---

## Technologies

* R Programming
* tidyverse
* ggplot2
* caret
* Machine Learning Algorithms

---

## Author

Mahomet Limenia Jean-Yves J. Keita
MBA – Supply Chain Management & Business Analytics
Université Laval

