# variable_selection_optimization
This project explored two ways to solve the problem of variable selection using optimzation with gurobi and LassoCV packages. 

Other contributors: Sahitya Vijayanagar, Brent Hensley, Archit Patel

## Problem and Objectives
This project explored two ways to solve the problem of variable selection that minimize an error metric:
1. Direct Variable Selection through Optimization - Mixed Integer Quadratic Programs
2. Regularization - LASSO

## Method 1: Mixed Integer Quadratic Programs (MIQP)
- Decision variables: continuous variables 𝑥𝑖, binary variables 𝑧𝑖
- Objective function: Minimize sum-of-squared error between the true dependent variable and the product of selected coefficients and their respective variables.
- Constraints:
- 1. Number of selected variables equals to k
- 2. Controlling if a variable is selected or not using 𝑧𝑖 (binary)

## Method 2: 
- using the Lasso CV package, more can be seen in the report pdf file above
- minimizes beta by finding optimal values for lambda (regularization parameter)

## Conclusion:
- If advanced tools and equipment with high computational abilities are inplace, we recommend using the MIQP method for variable selection. 
- If not, using Lasso for variable selection is still an effective method that generates a low sum squared error.
