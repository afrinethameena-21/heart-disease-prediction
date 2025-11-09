ouse Price Prediction using Machine Learning

This project demonstrates how to build a machine learning model to predict house prices based on various property features. Accurate house price prediction is essential in the real estate industry to make informed decisions for buyers, sellers, and investors.

Dataset

The model is trained on a dataset containing 2,919 records and 13 features, including:

MSSubClass: Dwelling type

MSZoning: Zoning classification

LotArea: Lot size in square feet

LotConfig: Lot configuration

BldgType: Type of dwelling

OverallCond: Overall condition rating

YearBuilt: Year of construction

YearRemodAdd: Remodel year

Exterior1st: Exterior covering

BsmtFinSF2: Type 2 finished basement area

TotalBsmtSF: Total basement area

SalePrice: Target variable (price of the house)

Project Steps

Data Preprocessing

Handled missing values by filling with mean or dropping nulls.

Removed irrelevant columns such as Id.

Exploratory Data Analysis (EDA)

Visualized numerical features using correlation heatmaps.

Analyzed categorical features using bar plots to understand distributions.

Feature Encoding

Converted categorical variables into numerical format using One-Hot Encoding.

Train-Test Split

Split data into 80% training and 20% testing sets.

Model Training

Trained multiple regression models including:

Support Vector Regression (SVR)

Random Forest Regressor

Linear Regression

Model Evaluation

Evaluated models using Mean Absolute Percentage Error (MAPE).

SVR achieved the lowest MAPE (~0.18), making it the most accurate model.

Random Forest and Linear Regression also gave reasonable performance.

Insights

Ensemble learning techniques like Bagging and Boosting can further improve prediction accuracy.

Feature engineering and domain-specific transformations can enhance model performance.

Conclusion

This project highlights the end-to-end workflow of a regression machine learning problem: data preprocessing → feature engineering → model training → evaluation. It demonstrates that SVR is a strong candidate for predicting house prices, but other models like Random Forest can also provide competitive results.
