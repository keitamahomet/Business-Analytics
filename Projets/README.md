# 📊 Business Analytics & Data Science Projects

## 👤 Author
**Mahomet Limenia Jean-Yves J KEITA**  
MBA – Supply Chain Management & Business Analytics  
Université Laval – Canada  

This repository presents a collection of **data analytics, machine learning, and optimization projects developed in R** as part of my graduate studies in Business Analytics.

These projects illustrate the application of **data science techniques to real-world decision-making problems**, including descriptive analysis, predictive modeling, mathematical optimization, and database design.

---

# 📌 Project Objectives

The primary objective of these projects is to demonstrate practical competencies in:

- Data cleaning and transformation
- Exploratory data analysis
- Data visualization
- Machine learning modeling
- Mathematical optimization
- Database design and querying
- Data-driven decision support

These projects were developed using **R and modern data science libraries**, following reproducible analysis practices.

---

# 📊 Descriptive Analytics Projects

Descriptive analytics focuses on **understanding and summarizing data to identify patterns, trends, and insights**.

---

## 🌳 Quebec Tree Dataset Analysis

### Project Description
This project analyzes a public dataset containing information about **trees located in different areas across Quebec**. The objective is to understand the distribution of tree species and identify locations with the highest concentration of trees.

### Methodology

1. Data import and cleaning using R
2. Detection and treatment of missing values
3. Calculation of descriptive statistics:
   - Mean
   - Standard deviation
   - Minimum
   - Maximum
4. Grouped analysis by:
   - Tree species
   - Measurement position
5. Data visualization to explore patterns in the dataset

### Key Insights

The analysis helped identify:
- The most common tree species
- Areas with the highest tree density
- Variability in tree measurements

### Technologies Used

- R
- tidyverse
- dplyr
- readr
- ggplot2

---

## 🏪 Customer Traffic Analysis – "Chez Tony"

### Project Description

This project analyzes **customer traffic data from a retail store** to identify temporal patterns in customer visits.

Understanding these patterns allows businesses to optimize:
- Staffing levels
- Operational planning
- Resource allocation

### Methodology

The analysis involved:

1. Data transformation into **tidy format**
2. Creation of time-based variables
3. Aggregation of customer counts by:
   - Hour
   - Day
   - Week
4. Visualization of traffic patterns using data visualization techniques

### Key Insights

The results identified:

- Peak customer hours
- High-traffic days
- Weekly patterns in store attendance

These insights support **operational decision-making in retail environments**.

### Technologies Used

- R
- tidyverse
- lubridate
- ggplot2

---

## 🌦 Weather Impact on Employee Activity

### Project Description

This project explores the relationship between **weather conditions and employee activity levels** by combining two datasets:

- Weather data from **Environment Canada**
- Employee connection/activity data

### Methodology

The analysis involved several steps:

1. Importing and cleaning multiple CSV datasets
2. Managing missing values
3. Feature engineering:
   - Weather condition indicators
   - Weekend indicator
   - Critical period variable
4. Merging datasets using joins
5. Comparative analysis and visualization

### Key Insights

The analysis revealed correlations between:

- Weather conditions
- Employee activity patterns

This type of analysis can help organizations understand **external factors affecting productivity or system usage**.

### Technologies Used

- R
- tidyverse
- dplyr
- ggplot2

---

# 🤖 Predictive Analytics Projects

Predictive analytics focuses on **using historical data to predict future outcomes or behaviors**.

---

## 🛒 Sales Analysis and Weather Impact (Willmart)

### Project Description

This project analyzes **sales data for a product at Willmart** and investigates whether weather conditions influence sales performance.

### Methodology

The project included the following steps:

1. Data cleaning and preparation
2. Integration of sales data with weather data
3. Exploratory data analysis to identify trends
4. Customer behavior segmentation using **K-means clustering**
5. Determination of the optimal number of clusters using the **Elbow Method**

### Key Insights

The clustering analysis revealed **distinct sales patterns associated with specific weather conditions**.

This type of analysis can support:

- Demand forecasting
- Inventory planning
- Marketing strategies

### Technologies Used

- R
- tidyverse
- cluster
- ggplot2

---

## 🌍 Greenhouse Gas Emissions Prediction

### Project Description

This project focuses on predicting **annual greenhouse gas emissions for companies in Quebec** using supervised machine learning models.

### Methodology

The modeling process involved:

1. Data preprocessing
2. Encoding categorical variables
3. Feature selection
4. Model training using multiple algorithms
5. Model evaluation using performance metrics

### Machine Learning Models Tested

- K-Nearest Neighbors (KNN)
- Neural Networks
- Random Forest

### Evaluation Metrics

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² (Coefficient of Determination)

### Results

Among the tested models, **KNN achieved the best balance between predictive accuracy and model stability**.

### Technologies Used

- R
- caret
- randomForest
- neuralnet

---

# 🧠 Prescriptive Analytics (Optimization)

Prescriptive analytics focuses on **using mathematical models to determine optimal decisions under constraints**.

---

## 💰 Multi-Period Investment Optimization

### Project Description

This project models an investment problem where an initial capital of **$550,000** must be allocated across different investment options over an **8-year horizon**.

### Constraints

- Investments have fixed durations
- Funds cannot be withdrawn before maturity
- Borrowing is not allowed
- Funds can be reinvested after maturity

### Objective

Maximize the final capital value at the end of the investment horizon.

### Results

The optimization model produced an **optimal investment strategy resulting in a final capital of $612,612**.

### Technologies Used

- R
- CVXR
- GLPK solver

---

## 🏭 Production – Sales – Inventory Optimization

### Project Description

This project models a **production planning problem over four periods** for a coffee company.

### Constraints

- Production capacity
- Inventory holding costs
- Production costs
- Minimum contractual sales requirements

### Objective

Maximize total profit across the planning horizon.

### Outcome

The optimization model identifies the optimal quantities to:

- Produce
- Sell
- Store

### Technologies Used

- R
- CVXR
- Linear programming

---

## 📹 Camera Placement Optimization

### Project Description

This project solves a **combinatorial optimization problem** involving the placement of security cameras in a building.

The goal is to determine the **minimum number of cameras required to monitor all corridors**.

### Methodology

The problem was modeled using:

- Integer programming
- Graph-based representation
- Optimization solvers

### Additional Approaches Tested

- Random search
- Genetic algorithms

### Objective

Compare exact optimization techniques with heuristic approaches.

### Technologies Used

- R
- CVXR
- GLPK

---

# 🗄 Data Engineering Project

## Relational Database Design with SQLite

### Project Description

This project involved creating a **relational database from raw CSV datasets** containing information about companies, categories, types, and locations.

### Methodology

1. Data cleaning and validation
2. Creation of primary keys
3. Detection and removal of duplicates
4. Validation of referential integrity
5. Construction of a relational schema
6. Analytical SQL queries

### Technologies Used

- R
- DBI
- RSQLite
- SQL

---

# 🛠 Technical Skills Demonstrated

## Programming Languages

- R
- SQL

## Data Analysis

- Data Cleaning
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Data Visualization

## Machine Learning

- K-Nearest Neighbors
- Random Forest
- Neural Networks
- Clustering (K-means)

## Optimization

- Linear Programming
- Integer Programming
- Mathematical Modeling
- Combinatorial Optimization

## Data Tools & Libraries

- tidyverse
- ggplot2
- caret
- CVXR
- RSQLite

---

# 📈 Career Focus

These projects reflect my interest in applying **data analytics to operations and supply chain management**.

My professional interests include:

- Supply chain analytics
- Demand forecasting
- Operational optimization
- Data-driven decision systems
- Business intelligence

---

💡 This repository is part of my **Data Analytics and Supply Chain Analytics portfolio developed during my MBA at Université Laval**.
