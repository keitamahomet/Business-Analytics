# Weather, Remote Work Activity and Exceptional Period Analysis

## Project Overview

This project analyzes the relationship between **weather conditions, employee activity, and exceptional periods** using hourly data.

The objective is to evaluate whether **weather conditions influence remote work behavior** and whether **exceptional events (such as crisis periods between 2020 and 2021)** have affected employee activity levels.

Employee activity is measured indirectly through **server connection logs**, which track when employees upload code, run tests, or interact with the company’s development server.

This project was completed as part of the **MQT7021 – Business Analytics course** in the **MBA in Business Analytics program at Université Laval**.

---

# Dataset

This project combines **two datasets**:

### 1 Weather Data

Hourly weather data from **Environment Canada**.

These datasets include information such as:

- Date and time
- Temperature
- Weather conditions (rain, snow, fog, etc.)

The files are stored in multiple CSV files located in:
data/meteo_log/env_can/envCanYqb_51457_hourly/


Key variables used:

- Date/Time
- Year
- Month
- Day
- Time
- Temperature (°C)
- Weather description

---

### 2 Employee Server Connection Data

This dataset contains server connection logs for **four remote software developers** employed by the company since **2017**.

Server connections occur when employees:

- deploy code
- run tests
- upload or download data
- interact with development servers

The dataset is stored in:
data/meteo_log/logged_all.csv

Each record represents a **connection event** associated with a specific employee.

---

# Objectives

The main objectives of this project are:

1. Import and combine multiple weather data files.
2. Clean and preprocess the weather dataset.
3. Clean the employee server connection logs.
4. Identify **good weather hours**.
5. Identify **exceptional periods (2020–2021)**.
6. Merge weather data with employee activity data.
7. Analyze whether:
   - weather conditions affect employee activity
   - exceptional periods affect connection behavior
8. Visualize patterns in employee activity.

---

# Methodology

The analysis was performed using **R** and the **tidyverse ecosystem**.

Main packages used:

- tidyverse
- lubridate
- dplyr
- ggplot2
- readr

---

# Data Processing

## 1 Loading Weather Data

Weather data is stored in **multiple CSV files**.

All files are loaded automatically using:

- `list.files()`
- `map()`
- `read_csv()`
- `reduce()`

Only the relevant columns were retained.

The dataset was then sorted by **date and time** to ensure correct chronological order.

---

## 2 Diagnosing Import Issues

Some files generated **warnings during import**.

The `problems()` function was used to identify:

- rows with inconsistent columns
- parsing issues

These issues were investigated to determine whether they were actual errors or data formatting inconsistencies.

---

## 3 Cleaning Weather Data

The dataset was cleaned by:

- identifying missing values
- replacing missing values using previous observations
- filling initial missing values using the first available observation

The `fill()` function from **tidyverse** was used for this step.

Only observations between **8:00 AM and 7:00 PM** were retained because employees only connect to the server during working hours.

---

## 4 Employee Connection Data

The employee connection dataset was imported and transformed into **tidy format**.

Each observation includes:

- date
- hour
- employee ID
- connection activity

Employee IDs were converted into integer values.

---

# Feature Engineering

Two additional variables were created.

---

## Good Weather Indicator

A new boolean variable was created to identify **good weather hours**.

An hour is considered **good weather** if:

- temperature ≥ 18°C
- weather conditions do not include:
Snow
Rain
Fog
Thunderstorm
Drizzle
Ice
Freezing


The `str_detect()` function was used to detect these conditions.

---

## Exceptional Period Indicator

A boolean variable named **exception** identifies hours within exceptional periods.

Two critical periods were defined:

- March 2020 – June 2020
- December 2020 – March 2021

These periods correspond to exceptional operational conditions.

---

# Data Integration

Weather data and employee connection data were merged using a **join operation**.

The join was designed to ensure that **no employee activity data was lost** during the merge.

The resulting dataset contains:

- weather information
- employee connection events
- good weather indicator
- exceptional period indicator

---

# Data Visualization

Visualizations were created using **ggplot2** to analyze patterns in employee activity.

The graphs allow us to evaluate:

- differences between employees
- differences between weekdays and weekends
- the impact of good weather
- the impact of exceptional periods

Trend lines were added to better observe changes in behavior over time.

---

# Technologies Used

- R
- tidyverse
- dplyr
- readr
- lubridate
- ggplot2
- R Markdown

---

# Project Structure
Weather_Employee_Activity_Analysis
│
├── README.md
├── weather_employee_analysis.Rmd
├── weather_employee_analysis.html
│
└── data
└── meteo_log
├── env_can
│ └── envCanYqb_51457_hourly
│ └── multiple_csv_files
│
└── logged_all.csv


---

# Skills Demonstrated

- Data integration from multiple sources
- Handling large collections of files
- Data cleaning and preprocessing
- Missing data handling
- Feature engineering
- Time series data analysis
- Data visualization
- Business analytics

---

# Author

Mahomet Limenia Jean-Yves J. Keita  
MBA – Supply Chain Management & Business Analytics  
Université Laval – Québec, Canada

