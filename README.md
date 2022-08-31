# Advanced Regression Assignment
> The aim of this project is to build a regression model with regularisation to predict the actual prices of house, given the dataset of previous sale of houses in Australia.

## Problem Statement
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.

The company is looking at prospective properties to buy, to enter the market. A regression model with regularisation is required in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:
- Which variables are significant in predicting the price of a house?
- How well those variables describe the price of a house?

## Business Goal
We should build a model to predict the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns.

## Conclusions
Ridge Model:
- Optimal value of lambda for Ridge regression is 0.2
- Train and Test R2 values are 0.894 and 0.876

Lasso Model:
- Optimal value of lambda for Lasso regression is 0.0001
- Train and Test R2 values are 0.890 and 0.874

Even though R2 values for Ridge and Lasso models are similar, we are preferring Lasso Model as few of the co-efficients are pushed to zero.

Top 10 variables that are significant in predicting the price of a house obtained from Lasso regression are:
- GrLivArea (0.427307)
- Exterior1st_BrkComm (-0.142601)
- TotalBsmtSF (0.132262)
- ExterQual_Fa (-0.114256)
- KitchenAbvGr (-0.100688)
- Functional_Maj2 (-0.096034)
- GarageCars (0.085781)
- LotArea (0.082234)
- Functional_Sev (-0.079253)
- ExterQual_TA (-0.078359)

## Libraries Used
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- sklearn
- statsmodels

## Acknowledgements
Coding references used from the following web-sites
- https://www.machinelearningplus.com/
- https://stackoverflow.com/
- https://www.geeksforgeeks.org/
- https://www.analyticsvidhya.com/
