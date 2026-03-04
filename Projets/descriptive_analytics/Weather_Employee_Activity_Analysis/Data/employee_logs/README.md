# Employee Server Connection Logs

## Overview

This file contains the **server connection activity logs of employees** used in the project:

**Weather and Remote Work Activity Analysis**

The dataset records when employees connect to the company server during working hours.  
These connections occur when employees perform activities such as:

- uploading code
- running tests
- interacting with development tools
- accessing shared project resources

The purpose of this dataset is to analyze **employee activity patterns over time** and study whether external factors such as **weather conditions or exceptional periods** influence remote work behavior.

---

## File

`logged_all.csv`

This dataset contains records of **server connections for four employees** who have been working remotely since **2017**.

Each observation represents a **connection event** made by an employee.

---

## Variables

The dataset contains the following key variables:

- **date**  
  Date of the connection.

- **hour**  
  Hour of the connection.

- **employee_id**  
  Identifier of the employee.

- **activity / connection indicator**  
  Indicates that a server interaction occurred.

---

## Use in the Analysis

This dataset is combined with **hourly weather data from Environment Canada** to study:

- employee activity patterns
- differences between employees
- variations in activity depending on the day or week
- potential impact of weather conditions
- impact of exceptional periods (e.g., 2020–2021)

The data is processed and analyzed using **R**, primarily with the following packages:

- tidyverse
- dplyr
- lubridate
- ggplot2

---

## Author

Mahomet Limenia Jean-Yves J. Keita  
MBA – Supply Chain Management & Business Analytics  
Université Laval – Québec, Canada
