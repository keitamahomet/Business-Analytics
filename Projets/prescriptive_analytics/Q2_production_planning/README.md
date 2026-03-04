# Production Planning Optimization

## Objective

This project models a production planning problem for a coffee company that produces ground coffee for a restaurant chain.

The goal is to maximize total profit over a four-month period while considering production capacity, inventory costs and market demand.

## Model Description

The model determines:

* monthly production quantities
* inventory levels
* sales quantities

Subject to constraints such as:

* production capacity limits
* inventory costs
* minimum purchase commitments
* maximum sales limit

## Optimization Method

The problem is formulated as a **linear programming model in compact form** and solved using the GLPK solver within the CVXR framework.

## Technologies

* R
* CVXR
* Linear Programming

