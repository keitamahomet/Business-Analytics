# Optimization and Mathematical Programming – Camera Placement & Investment Models

## Overview

This project explores the application of mathematical programming and combinatorial optimization to solve complex decision-making problems. The analysis was conducted in **R** using the **CVXR optimization framework** and additional algorithms to solve both linear and integer programming models.

The project contains three main optimization problems involving financial investment planning, production planning, and a graph-based surveillance optimization problem. The objective is to model these real-world problems mathematically and solve them using optimization techniques.

According to the project instructions, the analysis must be fully reproducible and implemented using **R Markdown**, with all code and results compiled into HTML reports. 

---

## Problem 1 – Investment Optimization

### Objective

The first problem focuses on determining the best strategy to reinvest **$550,000** obtained from selling a patent. The goal is to maximize the total capital available after **8 years**, considering several investment opportunities with different durations and interest rates.

### Approach

A **linear programming model** is formulated to decide:

* when to invest the available capital
* how much money to allocate to each investment option
* how cash flows evolve over time

### Key Constraints

* Investments must remain locked for their full duration
* Each investment option becomes available at a specific time
* Only safe investments are allowed (no borrowing)

### Tools Used

* R
* CVXR optimization package
* GLPK solver

---

## Problem 2 – Production Planning Optimization

### Objective

The second problem models a production planning scenario for a coffee company that produces and sells ground coffee to restaurants.

The goal is to **maximize total profit over four months** by deciding:

* production quantities
* inventory levels
* sales quantities

### Key Constraints

* production capacity: 81 kg per month
* storage cost: $2 per kg per month
* production cost: $3 per kg
* minimum demand: 55 kg per month
* maximum total sales: 312 kg

### Method

The problem is formulated as a **compact linear programming model** and solved using the GLPK solver.

---

## Problem 3 – Camera Placement Optimization

### Objective

The third problem involves determining the **minimum number of surveillance cameras** required to monitor all corridors in a building.

Corridors and intersections are represented as a **graph**, where:

* nodes represent intersections or corridor turns
* edges represent corridors
* cameras placed on nodes monitor adjacent corridors

The objective is to **cover all corridors using the smallest possible number of cameras**.

### Mathematical Formulation

This problem is formulated as an **integer programming model** where:

* decision variables determine whether a camera is placed at a given node
* constraints ensure every corridor is monitored
* the objective minimizes the total number of cameras installed

### Algorithms Implemented

Three approaches are used to solve the problem:

1. **Integer Programming (Exact Solution)**

   * solved with CVXR
   * GLPK_MI solver

2. **Random Search Algorithm**

   * generates candidate solutions
   * iteratively improves feasible solutions

3. **Genetic Algorithm**

   * implemented with the **GA package**
   * uses evolutionary strategies to find near-optimal solutions

Both heuristic algorithms ensure that the returned solutions remain feasible.

---

## Key Concepts Applied

This project demonstrates several important concepts in analytics and operations research:

* Linear Programming
* Integer Programming
* Mathematical Optimization
* Combinatorial Optimization
* Graph-based Optimization
* Heuristic Algorithms
* Genetic Algorithms
* Decision Modeling

---

## Technologies Used

* R
* R Markdown
* CVXR
* GLPK / GLPK_MI
* GA package
* Data visualization tools in R

---

## Key Skills Demonstrated

* Mathematical modeling
* Optimization problem formulation
* Algorithm design
* Heuristic search methods
* Data analysis and visualization
* Reproducible research using R Markdown

---

## Author

Mahomet Limenia Jean-Yves J. Keita
MBA – Supply Chain Management & Business Analytics
Université Laval

