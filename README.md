# Wine-quality-prediction
This repository contains the code and resources for a wine quality prediction project. This project aims to build a predictive model that can estimate the quality of wines based on physicochemical features. The project utilizes machine learning techniques and statistical analysis to achieve this objective.

Wine Quality Prediction Using Regression  
 
The two datasets are related to red and white Portuguese "Vinho Verde" wine variants. For more details, consult http://www.vinhoverde.pt/en/ or the reference [Cortez et al., 2009]. Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables are available (e.g. there is no data about grape types, wine brands, wine selling prices, etc.).  
These datasets can be viewed as classification or regression tasks. The classes are ordered and not balanced (e.g. there are many more normal wines than excellent or poor ones).  
This dataset is available from the UCI machine learning repository, https://archive.ics.uci.edu/ml/datasets/wine+quality 
 
Content  
•	Input variables (based on physicochemical tests): 1 - fixed acidity 2 - volatile acidity 3 - citric acid 4 - residual sugar 5 - chlorides 6 - free sulfur dioxide 7 - total sulfur dioxide 8 - density 9 - pH 10 - sulphates 11 - alcohol  
 
•	Output variable (based on sensory data): 12 - quality (score between 0 and 10) 
 
Questions that can be answered from the following model/ Project  
 
1.	What is the distribution of the wine quality scores? 
It can be observed that maximum red wine samples have a quality score of 6, with 5 following close behind, and the least number of wines have a quality score of 4. While in the white wine samples maximum has a quality score of 6, the least has a quality score of 4 and then 8. 
 
2.	What are the relationships between the different features? 
The correlation matrices plotted in the code can observe the relationship between the various features.  
 
3.	Are there any outliers in the data?  
There are no outliers in the red wine dataset, and the white wine data set does contain 
outliers, which are removed from the dataset.  
 
4.	What are the most essential features for the linear regression model? 
The top essential features of linear regression are density sulfates, volatile acidity, chlorides, etc. 
 
5.	What is the accuracy of the linear regression model? 
For Red Wine  
Training Accuracy = 0.3509850 
Testing Accuracy = 0.3893367 
 
For White Wine  
Training Accuracy = 0.2602418 
Testing Accuracy = 0.2556944 
  
6.	What is the MSE of the linear regression model? 
0. 5659548 for red wine and 0.7268164 for white wine. 
 
7.	What is the R-squared of the linear regression model? 
0.2556944 for white wine and 0.3893367 for red wine.  
 
8.	How can you improve the performance of the linear regression model? 
Hyperparameter Tuning: Tune the hyperparameters of the Linear Regression model, such as the regularization strength (alpha in Ridge and Lasso) or the learning rate (if using a gradient descent-based variant). 
 
Feature Scaling: Apply feature scaling to standardize or normalize the features. Standardization ensures that all features have the same scale, which can help the model converge faster. 
 
Polynomial Regression: Consider using Polynomial Regression to capture non-linear relationships between features and the target variable. This can be an extension of Linear Regression. 
 
9.	What are the limitations of the linear regression model? 
Linearity Assumption: Linear Regression assumes a linear relationship between the independent and dependent variables. The model's predictions may be inaccurate if the true relationship is not linear. 
 
Sensitivity to outliers: Linear regression is sensitive to outliers in the data. Outliers can have a disproportionate impact on a model's coefficients and predictions, causing the model to be less accurate. 
 
Independence Assumption: Linear regression assumes that the errors (residuals) are 
independent. If there is autocorrelation (correlation between the residuals at different time points in the time series data) or heteroscedasticity (different degrees of variance in the residuals), the model assumptions are violated. 
 
Limited to linear relationships: Without feature engineering or polynomial regression extensions, linear regression cannot capture complex non-linear relationships between independent and dependent variables. Other models, such as decision trees or neural networks, may better suit this situation. 
 
10. What are the implications of your findings for the real-world problem? 
Wineries can use these predictions to position their wines in the market strategically. They can highlight features leading to higher quality and market their products accordingly. 
 
 
 
 
