# Surprise Housing
> Advanced regression on predicting house price


## Table of Contents
1. [Problem Statement](#section1)<br>    
2. [Data Loading and Description](#section2)<br>
3. [Data cleaning](#section3)<br>
4. [Feature Engineering](#section4)<br>
5. [Exploratory Data Analysis](#section5)<br>
    5.1 [Univariate Analysis on numerical data](#section501)<br>
    5.2 [Bivariate Analysis on numerical data](#section502)<br>
    5.3 [Analysing relationship between categorical data](#section503)<br>
6. [Data Preparation](#section6)<br>
   6.1 [Splitting data into trainset and testset](#section601)<br>
   6.2 [Rescaling the features](#section602)<br>
   6.3 [Splitting into X_train and y_train on training dataset](#section603)<br>
7. [Model Building and Evaluation](#section7)<br>
   7.1 [Linear Regression](#section701)<br>
8. [Applying Regularisation Technique](#section8)<br>   
   8.1 [Ridge](#section702)<br>
   8.2 [Lasso](#section703)<br>
9.  [Inferences](#section9)<br>
10. [Assignment Part II](section10)<br>

1. Problem Statement

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

- Which variables are significant in predicting the price of a house
- How well those variables describe the price of a house.

### Business Goal 

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Conclusions
- __Optimal value of Lambda for Ridge Regression is 10__.
- __Optimal Value of Lambda for Lasso is 0.001__.
- Variables that play important role in predicting house price are.
  - OverallQual_9, OverallQual_10 , Neighborhood_StoneBr, Neighborhood_NridgHt, Neighborhood_NoRidge, OverallQual_8,        Neighborhood_Crawfor , RoofMatl_WdShngl, GrLivArea,      GarageYrBlt_2009.0, SaleType_New, BsmtExposure_Gd,  Exterior1st_BrkFace, OverallCond_9, LotConfig_CulDSac  
  
  - When we take our independent variable with respect ro target variable,
  - SalePrice increase by 2.525070 when we have OverallQual_9.
  - An increase in unit of the feature OverallQual_9affects thesale price by 2.439683.
  - If  neighbourhood is Neighborhood_StoneBr saleprice has an effect of 1.714167.
  - If neighbourhood is Neighborhood_Crawfor then sale price would increase by 1.371202.
  - When the material of roof provides a good factor in house sales then if roof material is Wood Shingles sale price would increase by    1.355345.
  - when living area Sq.feet increases by a unit then sale price of house would increase by 1.300925.
  - When the ouse has a garage and built in the year 2009, then  house price would increase by 1.297683.
  
  - __R-Squared Value__
  - Ridge Train : 0.91
  - Ridge Test  : 0.83
  - Lasso Train : 0.91
  - Lasso Test  : 0.83


## Technologies Used
- Python
## Tools used
- Jupyter notebook


## Acknowledgements
This project was done as an assignment for Executive PG programme in Machine Learning and Artificial Intelligence - IIIT Bangalore & upGrad


