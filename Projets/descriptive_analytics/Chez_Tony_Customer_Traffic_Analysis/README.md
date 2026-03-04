# Customer Traffic Analysis – Chez Tony

## Project Overview

This project analyzes customer traffic data from **Tony's high-tech locksmith shop**, a business specialized in **biometric smart locks and intelligent security systems**.

Tony records the number of customers entering the store **every hour of every business day**. After one month of operation, he wants to better understand customer behavior and identify patterns in store traffic.

The objective of this project is to transform and analyze the data in order to provide **insights that support operational and staffing decisions**.

This project was completed as part of the **MQT7021 – Business Analytics course** in the **MBA in Business Analytics program at Université Laval**.

---

# Dataset

The dataset contains hourly records of customer visits to the store.

The store operates:

- Monday to Friday
- From **9:00 AM to 6:00 PM**

The dataset is stored in:
data/chezTony.xlsx

Each observation represents:

- a **date**
- an **hour**
- the **number of customers**

---

# Objectives

The main objectives of this project are:

1. Import the Excel dataset directly using **R**.
2. Transform the dataset into **tidy format**.
3. Create new time-based variables:
   - Day of the week
   - Week number
4. Analyze customer traffic patterns.
5. Visualize customer traffic across:
   - hours of the day
   - days
   - weeks

---

# Methodology

The analysis was conducted using **R** and the **tidyverse ecosystem**.

## 1 Data Import

The dataset was imported directly from the Excel file using the **readxl** package.

A **relative path** was used to ensure reproducibility.

The first three rows of the dataset were displayed to verify that:

- the variables were correctly imported
- no information was lost during the import process

---

## 2 Data Cleaning and Transformation

The original Excel file is not in a format that is convenient for analysis.

Therefore, the dataset was transformed into **tidy format**, where each observation contains:

- the **date**
- the **hour**
- the **number of customers**

This transformation enables easier manipulation and analysis of the data.

---

## 3 Time Variables

Additional variables were created using the **lubridate** package:

### Day of the Week

The function `wday()` was used to generate labels representing the day of the week.

Examples:

- Mon
- Tue
- Wed
- Thu
- Fri

Weekends were excluded since the store is closed.

### Week Number

The function `week()` was used to compute the number of weeks since the beginning of the year.

This allows analysis of **customer traffic trends over time**.

---

# Data Visualization

Visualizations were created using **ggplot2** to help Tony understand customer traffic patterns.

## Customer Traffic by Hour and Day

A visualization was created to show how customer visits vary:

- across different hours
- across weekdays

This helps identify **low-traffic opening hours or closing hours**.

---

## Customer Traffic Over Time

Two additional visualizations were created:

### Daily Customer Traffic

This visualization shows how customer visits evolve **day by day**.

### Weekly Customer Traffic

This visualization aggregates visits **week by week** to reveal longer-term patterns.

A **linear regression trend line** was added using:
geom_smooth(method = "lm", se = FALSE)


This helps Tony evaluate whether customer traffic is increasing over time.

---

# Technologies Used

- R
- tidyverse
- dplyr
- readxl
- lubridate
- ggplot2
- R Markdown

---

# Project Structure
Chez_Tony_Customer_Traffic_Analysis
│
├── README.md
├── EQ1_TP1_Q2_chezTony_analyse_1.Rmd
├── EQ1_TP1_Q2_chezTony_analyse_1.html
│
└── data
└── chezTony.xlsx


---

# Skills Demonstrated

- Data import from Excel
- Data cleaning and transformation
- Tidy data formatting
- Time series analysis
- Data visualization
- Business analytics for decision making

---

# Author

Mahomet Limenia Jean-Yves J. Keita  
MBA – Supply Chain Management & Business Analytics  
Université Laval – Québec, Canada
