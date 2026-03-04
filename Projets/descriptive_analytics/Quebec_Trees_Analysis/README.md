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


A **relative path** was used for reproducibility.  
The function `problems()` was used to verify if any parsing issues occurred during data import.

The first three rows of the dataset were displayed to verify the successful loading of the data.

---

# Missing Values Analysis

A systematic verification of missing values was performed for **all columns** in the dataset.

Particular attention was given to the following critical variables:

- `ID`
- `LATITUDE`
- `LONGITUDE`

These fields are expected to contain **no missing values**, since they are essential for identifying and locating trees.

Missing values were identified programmatically using tidyverse functions.

---

# Statistical Analysis

The statistical analysis focused on tree trunk diameter measurements recorded at **breast height (DHP)**.

The following statistics were calculated **by tree type**:

- Mean diameter
- Standard deviation
- Minimum diameter
- Maximum diameter

These statistics provide insights into the **size distribution of different tree species**.

---

# Extended Statistical Analysis

The same statistical measures were computed again, but this time grouping the data by:

- **Measurement position**
- **Tree type**

This allows comparison between different measurement methods and tree categories.

---

# Identifying Potential Locations for Tree Enthusiast Outings

To determine the most suitable locations for a group outing, the dataset was filtered to include only:

- **Public properties**

The number of trees was then counted by **topographical location (address)**.

Additionally, the number of:

- **Deciduous trees**
- **Coniferous trees**

was calculated for each location.

Finally, the **10 locations with the highest number of trees** were identified as potential destinations for the group outing.

---

# Technologies Used

- R
- tidyverse
- dplyr
- readr
- ggplot2

---

# Key Skills Demonstrated

- Data Cleaning and Transformation
- Exploratory Data Analysis (EDA)
- Handling Missing Values
- Statistical Analysis
- Data Aggregation and Grouping
- Reproducible Data Analysis using R Markdown

---

# Author

Mahomet Limenia Jean-Yves J. Keita  
MBA – Supply Chain Management & Business Analytics  
Université Laval – Québec, Canada
