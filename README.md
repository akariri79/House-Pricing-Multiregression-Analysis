Boston House Pricing: Multivariable Regression & Valuation Model
📌 Project Overview

This project applies multivariable linear regression to predict median house prices in Boston suburbs using multiple housing market and environmental variables.
It demonstrates the end-to-end data science workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and visualization.

🎯 Problem Statement

Real estate pricing is influenced by multiple socio-economic and geographic factors.
The goal of this project is to:

Understand the key drivers of Boston housing prices

Build a regression model that can predict house values

Provide insights that can guide property valuation and investment decisions

📂 Dataset

Source: Boston Housing Dataset (scikit-learn)

Instances: 506

Features: 13 numerical features (e.g., average number of rooms, crime rate, proximity to employment centers)

Target Variable: Median value of owner-occupied homes (MEDV) in $1000's

🛠 Tech Stack

Python (3.14)

Libraries:

Data Analysis: Pandas, numpy

Visualization: Matplotlib, Seaborn, Plotly

Modeling: Scikit-Learn

Jupyter Notebook for development & documentation

📊 Project Workflow

Data Loading & Cleaning

Loaded dataset from sklearn.datasets

Checked for null values and data types

Exploratory Data Analysis (EDA)

Visualized distributions and correlations

Identified most influential features

Feature Engineering

Normalized/standardized numerical features

Checked multicollinearity

Applied **logarithmic transformation to the target variable** (MEDV) to reduce heteroscedasticity and improve model performance

Model Training

Applied Multiple Linear Regression

Split dataset into training and test sets

Model Evaluation

Evaluated performance using R² and residual plots

Applying a log transform on target variable (MEDV) significantly improved model fit and error distribution

Visualization

Scatter plots of predicted vs. actual values

Residual analysis

📈 Key Insights

Top Predictors:

Average number of rooms per dwelling (RM)

Lower crime rate (CRIM)

Proximity to employment centers (DIS)

Model Performance:

R² Score before transform: 0.750 (Training), 0.671 (Test)

R² Score after transform: 0.793 (Training), 0.745 (Test)

MAE before transform: 4.06

MAE after transform: 3.480

MSE before transform: 34.414

MSE after transform: 28.218

RMSE before transform: 5866.342

RMSE after transform: 5312.049

Interpretation:

Applying the **log transform** on MEDV significantly improved model fit and error distribution

Houses with more rooms and located in low-crime areas tend to have higher prices

Accessibility to job hubs is a significant factor
