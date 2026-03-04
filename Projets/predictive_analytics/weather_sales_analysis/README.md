# Weather Sales Analysis

## Overview
This project analyzes the relationship between product sales and weather conditions using historical retail and meteorological data.

The objective is to determine whether temperature and precipitation influence sales performance.

## Dataset
The dataset contains daily sales records combined with weather observations.

Main variables:
- date
- storeId
- itemId
- units sold
- temperature (max, min, avg)
- precipitation
- snowfall
- wind speed

## Methodology

### Data Cleaning
- Filtering relevant stores
- Handling missing values
- Converting units to metric system
- Feature transformation

### Exploratory Data Analysis
- Sales distribution by product
- Sales vs temperature
- Sales vs precipitation
- Monthly visualization using faceting

### Clustering
To identify patterns in sales behavior, k-means clustering was applied using:

- total sales
- maximum temperature
- precipitation

The optimal number of clusters was determined using the elbow method.

## Tools
- R
- tidyverse
- ggplot2
- stats (kmeans)

## Key Insights
- The most sold item shows strong variation across months.
- Temperature appears to influence sales patterns.
- Precipitation has weaker impact but may reduce sales in some periods.
