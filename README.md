# Predicting Used Car Prices with Regression Models

## Introduction

This project is an end-to-end machine learning task using a dataset of used cars. The goal is to build and compare three regression models for predicting the selling prices of used cars.

## Objectives

- Build Multiple Linear Regression, Decision Tree, and Random Forest models.
- Compare the models and evaluate their performance using appropriate regression metrics.

## Key Results

Overall, the most represented car brands in the dataset had relatively lower selling prices.

Random Forest was the best-performing model, achieving an R² score of 0.824 and the lowest MAE and RMSE among the three models.

Prediction errors were still relatively large. This may be associated with the limited number of vehicle characteristics available in the dataset and the presence of duplicate records.

## Dataset

The dataset was obtained from Kaggle and contains information about used vehicles from online listings. It has 8,128 records, with four predictor variables (`brand`, `km_driven`, `fuel`, and `owner`) and `selling_price` as the target variable.

The dataset had no missing values. However, it contained 1,678 duplicate rows, accounting for approximately 21% of the dataset.

[View the dataset on Kaggle](https://www.kaggle.com/datasets/ahmedfakhar123/used-car-price-prediction-dataset/data?select=Used_Car_Prices.csv)

## Exploratory Data Analysis

Maruti was the most represented car brand, followed by Hyundai and Mahindra. Most cars in the dataset were first-owner vehicles.

Luxury brands such as Mercedes-Benz, BMW, and Volvo had wider selling price ranges compared with less expensive brands.

## Methodology

Categorical features were transformed using one-hot encoding, while `km_driven` was standardized.

The dataset was split into 80% training data and 20% testing data.

Three regression models—Multiple Linear Regression, Decision Tree, and Random Forest—were trained and evaluated using R², MAE, and RMSE.

Prediction error analysis was then performed on the best-performing model to better understand its errors.

## Models and Evaluation

The three models were evaluated using R², MAE, and RMSE. The results are summarized below:

| Model | R² | MAE | RMSE |
|---|---:|---:|---:|
| Linear Regression | 0.778 | ₹216,466 | ₹381,605 |
| Decision Tree | 0.783 | ₹184,174 | ₹377,504 |
| Random Forest | 0.824 | ₹177,752 | ₹340,132 |

Random Forest achieved the best overall performance, with the highest R² and the lowest MAE and RMSE.

## Limitations

The dataset contains only four predictor variables, which limits the model's ability to distinguish between vehicles with similar recorded characteristics. Important factors such as manufacturing year, car model, engine size, transmission, and vehicle condition were not available.

The presence of duplicate records may also affect how well the evaluation results represent performance on completely unseen vehicles.

## Tools & Libraries

- **Python** — programming language
- **Jupyter Notebook** — development environment
- **Pandas** — data manipulation and analysis
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — preprocessing, model development, and evaluation
