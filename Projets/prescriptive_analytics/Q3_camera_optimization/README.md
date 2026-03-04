# Camera Placement Optimization

## Objective

This project determines the minimum number of surveillance cameras required to monitor all corridors of a building.

Corridors and intersections are represented as a **graph**, where nodes represent intersections and edges represent corridors.

Cameras placed at nodes can monitor adjacent corridors.

## Optimization Model

An **integer programming model** is formulated where:

* binary decision variables determine whether a camera is placed at a node
* constraints ensure that every corridor is monitored
* the objective minimizes the total number of cameras

## Algorithms Implemented

Three solution approaches are implemented:

1. Exact solution using Integer Programming
2. Random Search algorithm
3. Genetic Algorithm using the GA package

These approaches allow solving both small and large instances of the problem.

## Data

The model uses adjacency matrices representing building layouts.

Files included:

* tiny_problem_adjacency_matrix.rds
* large_problem_adjacency_matrix.rds

## Technologies

* R
* CVXR
* GLPK_MI
* GA package
* Graph optimization techniques

