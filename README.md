# Project 2 - Ames Housing Data and Kaggle Challenge
## Problem Statement
By conducting exploratory data analysis, data processing and modeling, the objective of this project is to build the best regression model, using the Ames Housing Dataset, to predict the price of a house at sale and will be scored by the Root Mean Squared Error.
<br>
<br>
The 2 data sets provided are a train set containing all the information in Ames Housing Project which will be used to build the model for prediction and a test set which has all the columns found in the train set except for the SalePrice column which we will be predicting. Excluding SalePrice and Id, the train dataset contains 2051 observations and 79 features and the test dataset contains 879 observations and 78 features. 
## Data dictionary
https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data
## Table of content
- [Problem Statement](#problem-statement)
- [EDA](#eda)
  * [Import libraries and load datasets](#import-libraries-and-load-datasets)
  * [Check for null](#check-for-null)
- [Data Cleaning](#data-cleaning)
  * [Summary of fixing null values](#summary-of-fixing-null-values)
  * [Check categorial features](#check-categorial-features)
  * [Check numerical features](#check-numerical-features)
- [Exploratory Visualizations](#exploratory-visualizations)
  * [Scatterplot](#scatterplot)
  * [Removing outliers](#removing-outliers)
  * [Histograms](#histograms)
  * [Boxplots](#boxplots)
  * [Feature engineering](#feature-engineering)
  * [Heatmap](#heatmap)
- [Pre-processing](#pre-processing)
- [Modeling](#modeling)
  * [Linear regression](#linear-regression)
  * [Kaggle score:](#kaggle-score-)
  * [Ridge regression](#ridge-regression)
  * [Lasso regression](#lasso-regression)
  * [Model comparison](#model-comparison)
- [Inferential Visualizations](#inferential-visualizations)
- [Business Recommendations](#business-recommendations)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>
## Executive summary
<p>To start things off, relevant libraries are imported and both datasets, train.csv and test.csv are loaded. Upon checking, it is observed that the train set contains 2051 observations and 81 features and the test set contains 879 observations and 80 features, short of the feature SalePrice which is what will be predicted.
</p>
<p>First step in exploratory data analysis is checking and handling null values. After null values are handled, categorical features are inspected and those with over 90% of values in the same category are removed. Same process is then carried out on numerical features. Using exploratory visualizations, outliers are then removed and feature engineering carried out.
</p>
<p>20 features with highest correlation to SalePrice are selected and pre-processing carried out for modeling. 3 models, linear, ridge and lasso regression models are used and ridge model is eventually selected for the lowest Root Mean Squared Error of 27091.35.
</p>

## Conclusion and summary
As observed from the coefficients from ridge model, the 5 features that add the most value to a home are 
1. Exter Qual: Exterior material quality
2. Kitchen Qual: Kitchen quality
3. Gr Liv Area: Above grade (ground) living area square feet
4. Neighborhood: Physical locations within Ames city limits
5. Overall Qual: Overall material and finish quality

The features that hurt the value of the home the most are
1. Age: Age of house
2. Full Bath: Full bathrooms above grade
3. TotRms AbvGrd: Total rooms above grade (does not include bathrooms)
4. Year Built: Original construction date
5. Bsmt Qual: Height of the basement

<p>According to the model, in order to increase the value, homeowners are highly recommended to use excellent quality materials for the exterior, kitchen and in overall. At the same time, houses in Stone Brook, Northridge Heights, North Ridge and Veenker with large ground living area can fetch the best price.
</p>
<p>Data shows that houses in Stone Brook, Northridge Heights, North Ridge and Veenker command the highest price in this city. Based on this information, with the highest potential to reach high price, these 4 neighborhoods are the most recommended for investment.
</p>
<p>This model ranked 30+ in private and 50+ in public leaderboard on Kaggle. Scoring is based on the model's prediction performance on unseen data. The top and bottom 5 features, except 1, that affect the prediction the most are all general features of a house so I would say it should perform fairly well when generalizing to other cities. The one most important data I would need from another city to make a comparable model would be Neighborhood since that is the one feature that would be most different and it is the 4th feature that adds most value to a house in my model.
</p>