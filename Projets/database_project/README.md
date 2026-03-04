# Database Analysis Report

## Overview

This directory contains the analytical report for the **Companies Relational Database Project**. The report documents the complete process of preparing the datasets, building the relational database, and executing SQL queries to extract insights.

The analysis is written using **R Markdown**, which allows the integration of code, explanations, and results in a single reproducible document.

The final report is compiled into **HTML format** so that the analysis can be easily viewed and shared.

---

## Files

### database_analysis.Rmd

This file contains the complete analysis written in **R Markdown**.

It includes:

* loading and inspecting the datasets
* cleaning and validating relational data
* preparing the tables for database creation
* connecting to the SQLite database
* executing SQL queries
* displaying query results and explanations

The R Markdown file combines:

* R code
* SQL queries
* explanations of the methodology
* output tables and visualizations

---

### database_analysis.html

This file is the compiled version of the R Markdown report.

It is the final report used to present the analysis and results. The HTML file contains:

* formatted explanations
* executed code results
* query outputs
* tables and visualizations

This file can be opened directly in a web browser.

---

## Reproducibility

To reproduce the analysis:

1. Open the project in RStudio.
2. Ensure the required packages are installed.
3. Run or knit the **database_analysis.Rmd** file.

Required packages include:

```r
readr
dplyr
DBI
RSQLite
```

---

## Purpose of the Report

The report demonstrates how to:

* prepare relational datasets
* ensure data integrity
* construct a SQLite database
* perform SQL queries within R
* present results in a reproducible analytical report

---

## Author

Mahomet Limenia Jean-Yves J. Keita
MBA – Supply Chain Management & Business Analytics
Université Laval

