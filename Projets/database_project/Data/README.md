# Dataset – Companies Database Project

## Overview

This directory contains the raw datasets used to build a relational database of companies located in the United States and Canada. The data will be integrated into a **SQLite relational database** and analyzed using SQL queries in R.

The objective of this dataset is to support the creation of an **integrity-preserving relational database**, ensuring proper entity and referential integrity between tables.

---

## Files Description

### Q1_categories.csv

This file contains the list of company categories.

Main variable:

* **category** – category assigned to each company.

This table will be used to define the categories available in the database.

---

### Q1_companies.csv

This dataset contains detailed information about companies.

Main variables include:

* **id** – unique identifier of the company
* **name** – company name
* **url** – company website
* **year_founded** – year the company was founded
* **full_time_employees** – number of employees
* **type** – company type
* **company_category** – category of the company
* **revenue_source** – source of revenue
* **business_model** – business model
* **location_id** – reference to the company location

This table represents the central entity of the database.

---

### Q1_locations.csv

This dataset contains information about company locations.

Main variables:

* **location_id** – unique identifier for the location
* **city** – city where the company operates
* **state** – state or province

This table allows companies to be associated with a geographic location.

---

### Q1_types.csv

This dataset defines the different types of companies.

Main variables:

* **type** – identifier of the company type
* **description** – description of the type

This table helps classify companies according to their type of organization.

---

## Data Usage

The datasets are loaded into R using the following command:

```r
library(readr)

data_cat <- read_csv("data/Q1_categories.csv")
data_com <- read_csv("data/Q1_companies.csv")
data_loc <- read_csv("data/Q1_locations.csv")
data_typ <- read_csv("data/Q1_types.csv")
```

The datasets are then cleaned and used to construct a **SQLite relational database** with properly defined primary keys and foreign key relationships.

---

## Purpose

These datasets support the following tasks:

* cleaning and validating relational data
* creating a SQLite database
* enforcing primary and foreign key constraints
* performing SQL queries to analyze company information
