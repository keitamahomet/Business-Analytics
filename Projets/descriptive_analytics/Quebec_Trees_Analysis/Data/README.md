# Dataset – Quebec Trees

## Overview

This folder contains the dataset used for the **Quebec Trees Analysis** project.

The data comes from the **open data portal of the City of Québec** and contains information about trees located throughout the city.

The dataset is used to analyze tree characteristics and identify locations with the highest concentration of trees.

---

## Data Source

City of Québec – Open Data Portal  
Tree Inventory Dataset (2025)

The original dataset includes information about tree species, locations, and physical measurements.

---

## File Description

vdq-arbrerepertorie.csv

This file contains the tree inventory data used in the analysis.

Each row represents a **single tree** recorded in the dataset.

---

## Variables

| Variable | Description |
|--------|-------------|
| ID | Unique identifier for each tree |
| TYPE_LIEU | Type of location where the tree is planted |
| NOM_LATIN | Latin name of the tree |
| NOM_FRANCAIS | French name of the tree |
| TYPE_ARBRE | Type of tree (deciduous or conifer) |
| DIAMETRE | Diameter of the trunk (cm) |
| POSITION_MESURE | Measurement position of the diameter |
| MULTI_TRONC | Indicates whether the tree has multiple trunks |
| DATE_PLANTE | Planting date |
| TYPE_PROP | Property type (public or private) |
| NOM_TOPOGRAPHIE | Address or topographic name |
| LATITUDE | Latitude coordinate |
| LONGITUDE | Longitude coordinate |

---

## Usage

The dataset is read in the analysis using the following relative path:

data/arbres_qc/vdq-arbrerepertorie.csv

The file is imported in R using the **read_csv()** function from the **readr** package.

---

## Notes

Some variables may contain missing values, particularly:

- planting dates
- diameter measurements

However, critical variables such as **ID, LATITUDE, and LONGITUDE** should not contain missing values.

---

## Author

Mahomet Limenia Jean-Yves J. Keita  
MBA – Supply Chain Management & Business Analytics  
Université Laval
