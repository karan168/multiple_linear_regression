This project demonstrates how to apply Multiple Linear Regression (MLR) using scikit-learn in Python. 
It includes both raw and standardized feature modeling and emphasizes interpreting regression outputs such as coefficients, R-squared, and p-values.
The model aims to predict a student's GPA based on SAT scores and a randomly generated feature Rand1,2,3
objective:
To build a multiple linear regression model that:
          1.Predicts GPA using SAT scores and a non-informative feature
          2.Evaluates model significance and goodness-of-fit using R² and adjusted R²
          3.Performs feature standardization
          4.Uses feature selection techniques to determine the significance of predictors
Dataset:
The dataset is loaded from a CSV file and contains the following columns:
          1.SAT: Standardized test scores
          2.Rand 1,2,3: A synthetic random feature
          3.GPA: Target variable representing Grade Point Average
Steps:
Data Loading & Exploration
     Load the dataset and check descriptive statistics.
Model Construction
     Define SAT and Rand 1,2,3 as independent variables.
     Use LinearRegression to fit the model and predict GPA.
Evaluation
     Calculate R² and Adjusted R² to assess model performance.
     Use f_regression to compute p-values for each feature.
Interpretation
     Summarize coefficients and statistical significance in a table.
     Conclude that SAT is a meaningful predictor, while Rand 1,2,3 is not.
Feature Scaling
     Apply StandardScaler from sklearn.preprocessing.
     Refit the regression model on the standardized features.
Final Summary Table
     Present bias and feature weight-post standardization

Conclusion
SAT is a statistically significant and meaningful predictor of GPA.
The random feature does not contribute meaningfully and could be discarded.
Standardization helps interpret the influence of features measured on different scales.
