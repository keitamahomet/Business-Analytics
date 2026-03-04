# Data Files – Camera Placement Optimization

## Overview

This directory contains the datasets used for the **Camera Placement Optimization** problem. The files represent building layouts in the form of **adjacency matrices**, which describe how corridors connect intersections, turns, and dead ends within a building.

Each dataset defines a different instance of the surveillance optimization problem.

---

## Data Description

The adjacency matrices represent a **graph structure**:

* **Rows and columns** represent intersections, corridor turns, or dead ends.
* A value of **1** indicates that two locations are connected by a corridor.
* A value of **0** indicates that no direct corridor exists between the two locations.

These matrices are **symmetric**, meaning that if location *i* is connected to location *j*, then location *j* is also connected to location *i*.

Diagonal values are ignored because they represent a node connected to itself.

---

## Files Included

### tiny_problem_adjacency_matrix.rds

A small instance of the camera placement problem used for testing and validating the optimization model and algorithms.

Characteristics:

* small number of nodes
* useful for debugging the model
* allows quick verification of feasibility and objective values

---

### large_problem_adjacency_matrix.rds

A larger instance of the camera placement problem designed to test the performance of the optimization model and heuristic algorithms.

Characteristics:

* larger graph
* more complex corridor network
* used to evaluate algorithm efficiency and scalability

---

## Usage

These datasets are loaded into R using the following command:

```r
adj_matrix <- readRDS("data/tiny_problem_adjacency_matrix.rds")
```

or

```r
adj_matrix <- readRDS("data/large_problem_adjacency_matrix.rds")
```

The adjacency matrix is then used as input for the optimization model that determines the minimum number of cameras required to monitor all corridors.

---

## Format

File format: **.rds**

The `.rds` format stores R objects and allows efficient loading of structured data directly into R environments.

---

## Author

Mahomet Limenia Jean-Yves J. Keita
MBA – Supply Chain Management & Business Analytics
Université Laval

