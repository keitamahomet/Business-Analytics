# Investment Optimization Model

## Objective

This project models an investment planning problem where a total capital of $550,000 must be reinvested across several financial options. The objective is to maximize the total capital available after eight years.

## Methodology

A **linear programming model** is formulated to determine:

* how much to invest
* when to invest
* which investment option to choose

Each investment has a specific:

* interest rate
* investment horizon
* availability year

The model ensures that funds remain invested for their full duration and that investments can only be made at specific times.

## Tools Used

* R
* CVXR optimization framework
* GLPK solver

## Output

The optimization model returns:

* the optimal investment allocation
* the final capital value
* solver status indicating optimality

