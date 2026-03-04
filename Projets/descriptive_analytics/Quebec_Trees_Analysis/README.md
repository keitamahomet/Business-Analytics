# Quebec Trees Analysis

## Project Context

This project analyzes a dataset of trees located in the city of **Québec**, using open data provided by the **Ville de Québec (2025)**.  

The objective of the analysis is to identify locations in Québec City with the **highest concentration of trees** in order to help organize a potential outing for a group of tree enthusiasts.  

Additionally, the analysis explores **statistical characteristics of trees by type**, which may be of interest to participants of the ADADQC group (Amateurs d'Arbres de Québec).

This project was completed as part of the **MBA in Business Analytics at Université Laval**.

---

# Dataset Description

The dataset contains detailed information about trees located throughout Québec City.

Each observation represents a **single tree** and includes the following variables:

| Variable | Description |
|--------|-------------|
| ID | Unique identifier for each tree |
| TYPE_LIEU | Type of location where the tree is planted |
| NOM_LATIN | Latin name of the tree |
| NOM_FRANCAIS | French name of the tree |
| TYPE_ARBRE | Type of tree (e.g., deciduous or conifer) |
| DIAMETRE | Diameter of the trunk in centimeters |
| POSITION_MESURE | Position where the diameter was measured |
| MULTI_TRONC | Boolean indicator of whether the tree has multiple trunks |
| DATE_PLANTE | Tree planting date (when available) |
| TYPE_PROP | Property type (public or private) |
| NOM_TOPOGRAPHIE | Address or topographical location |
| LATITUDE | Latitude coordinate |
| LONGITUDE | Longitude coordinate |

### Measurement Positions

Diameter measurements may correspond to different measurement positions:

- **DHP** — Diameter at breast height  
- **DHS** — Diameter at stump height  
- **M** — Mean diameter for multi-trunk trees

---

# Data Processing

The analysis was conducted using **R** and the **tidyverse** ecosystem.

## Data Import

The dataset was read using the `read_csv()` function from the **readr** package:

