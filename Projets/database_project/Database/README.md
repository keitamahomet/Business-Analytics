# Companies Relational Database (SQLite)

## Overview

This project presents the creation of a **relational database of companies in the United States and Canada** using **SQLite**. The database was built from several CSV datasets and structured to ensure proper **entity integrity and referential integrity** between tables.

The objective of this project is to design and implement a clean relational database that can support data analysis and SQL queries related to companies, their locations, categories, and organizational types.

---

## Database File

**companies_bd.sqlite**

This SQLite database contains all the cleaned and structured data integrated into relational tables.

The database can be opened using tools such as:

* DB Browser for SQLite
* R (using DBI and RSQLite packages)
* Python (sqlite3 library)

---

## Database Schema

The relational database is composed of four main tables:

### companies

Stores information about companies.

Key attributes:

* **id** – unique company identifier (Primary Key)
* name – company name
* url – company website
* year_founded – year of foundation
* full_time_employees – number of employees
* type – company type
* company_category – category of the company
* revenue_source – revenue source
* business_model – business model
* location_id – reference to the company location

---

### locations

Stores geographic information about company locations.

Attributes:

* **location_id** – location identifier (Primary Key)
* city – city where the company is located
* state – state or province

---

### categories

Stores company category classifications.

Attributes:

* **category** – category identifier (Primary Key)

---

### types

Stores company type classifications.

Attributes:

* **type** – type identifier (Primary Key)
* description – description of the company type

---

## Relationships

The database enforces several foreign key relationships:

* companies.location_id → locations.location_id
* companies.company_category → categories.category
* companies.type → types.type

These relationships ensure **referential integrity** between the tables.

---

## Example Queries

Example SQL queries that can be executed on the database:

### Companies founded between 1998 and 2001

```sql
SELECT name, url
FROM companies
WHERE year_founded BETWEEN 1998 AND 2001
ORDER BY name;
```

### Companies located in Oregon

```sql
SELECT companies.name, companies.url, locations.city, companies.year_founded
FROM companies
JOIN locations
ON companies.location_id = locations.location_id
WHERE locations.state = 'Oregon';
```

### Median founding year by category

```sql
SELECT company_category,
       COUNT(*) AS number_of_companies,
       AVG(year_founded) AS average_year
FROM companies
GROUP BY company_category;
```

---

## Technologies Used

* SQLite
* R
* DBI
* RSQLite
* readr
* SQL

---

## Skills Demonstrated

* Relational database design
* Data cleaning and preparation
* Entity integrity and referential integrity
* SQL querying
* Data integration from multiple sources

---

## Author

Mahomet Limenia Jean-Yves J. Keita
MBA – Supply Chain Management & Business Analytics
Université Laval

