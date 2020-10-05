# Housing-Price-Prediction

## Background
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them at a higher price.The company is looking at prospective properties to buy to enter the market.
The company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

## Objective and Goals
We are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for the management to understand the pricing dynamics of a new market.


## Dataset
The dataset is extracted from existing australian real estate market. It has many independent variables and a target variable 
The dataset and data dictionary can be downlaoded from (URL:https://drive.google.com/drive/folders/1PJUvh62LRWednJB40MAghkrQCIqGsPKu?usp=sharing)

## Tech Stack
- Preprocessing - Numpy and Pandas
- Visulatization - Matplotlib and Searborn
- Modelling - Sklearn (LinearRegression, Ridge and Lasso)
- Hyperparameter Tuning - Sklearn (GridsearchCV)

## Results
Ridge Regression Metrics
- Train r2 -0.91
- Test r2 - 0.89
  
Lasso Regression Metrics
- Train r2 - 0.91
- Test r2 - 0.89
  
Important Factors for the price prediction as per Lasso and ridge are
- GrLivArea
- OverallQual
- Exterior1st_others

The regularized regression(both Lasso and ridge) has a 2% error in prediction on test data as compared to 3% in OLS method.
Hence i would use regularizes model as compared to OLS for better accuracy.

Among Lasso and ridge i would choose Lasso as my final model even when the accuracy of both models are same because Lasso has less features as compared to ridge.As there are less variables, it is much simpler model. Simpler models are always better because of low varinace , high stability and genralizuibility.
