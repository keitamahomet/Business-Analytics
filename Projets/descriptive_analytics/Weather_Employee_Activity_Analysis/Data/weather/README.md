# Environment Canada Hourly Weather Data – Québec City

## Overview

This folder contains **hourly weather data for Québec City** obtained from **Environment and Climate Change Canada**.

The data is used in the project **Weather and Remote Work Activity Analysis**, where weather conditions are analyzed alongside employee server activity.

The objective is to determine whether **weather conditions influence remote work behavior and employee activity patterns**.

---

## Data Source

Environment and Climate Change Canada  
Hourly Climate Data

The data was downloaded and stored as **monthly CSV files**.

---

## File Structure

Each file follows the naming format:
en_climate_hourly_QC_7016293_MM-YYYY_P1H.csv

Where:

- **MM** = month  
- **YYYY** = year  
- **P1H** = hourly frequency  

Example:
en_climate_hourly_QC_7016293_01-2020_P1H.csv

This file contains **all hourly weather observations for January 2020**.

---

## Variables Used in the Analysis

Although the raw files contain many variables, the analysis focuses mainly on:

- **Date/Time**
- **Temperature (°C)**
- **Weather conditions**

These variables are used to create indicators such as:

- good weather conditions
- weather categories for analysis

---

## Data Processing

All weather files are automatically loaded in **R** using a loop that reads every CSV file in the folder.

Example:

```r
library(tidyverse)

files <- list.files(
  "data/meteo_log/weather",
  pattern = "\\.csv$",
  full.names = TRUE
)

weather_data <- files %>%
  purrr::map(readr::read_csv) %>%
  dplyr::bind_rows()
Notes

Some files may produce parsing warnings when imported using read_csv.
These warnings are checked using the problems() function and handled during data cleaning.

The dataset is later merged with employee server connection logs to analyze behavioral patterns.

Author

Mahomet Limenia Jean-Yves J. Keita
MBA – Supply Chain Management & Business Analytics
Université Laval – Québec, Canada
