# Wikipedia Page Views Prediction

## Overview

This script aims to predict the number of times the Wikipedia page of Machine Learning was read using two different time series forecasting models: Facebook Prophet and Neural Prophet. The dataset "wiki_machine_learning.csv" is used for this prediction task. The script involves data preprocessing, model training, and evaluation.

## Dataset Information

### Description

The dataset represents the count of how many times the Wikipedia page of Machine Learning was read during a specific period. The data is presented in CSV format with columns: date, count, lang, page, rank, month, and title. Null values in the count column are identified with 0.

### File

- **Dataset:** [wiki_machine_learning.csv]

## Script Structure

### 1. Data Loading and Preprocessing

- **Loading Data:** The script loads the dataset into a Pandas DataFrame.

- **Cleaning Data:** Null values in the count column are identified with 0 and removed during preprocessing. The date column is converted to datetime, and the count column is converted to numeric.

### 2. Facebook Prophet Model

- **Model Training:** A Facebook Prophet model is trained to predict the count of page views.

- **Hyperparameter Tuning:** The script explores different hyperparameter combinations using Bayesian Optimization.

- **Forecasting:** The model is used to make forecasts for the next 30 days.

### 3. Neural Prophet Model

- **Model Training:** A Neural Prophet model is trained to predict the count of page views.

- **Forecasting:** The model is used to make forecasts for the next 30 days.

### 4. Model Evaluation

- **Cross-Validation:** The script performs cross-validation to evaluate the models' performance over time.

- **Performance Metrics:** Various performance metrics, including Mean Percentage Error (MPE), are calculated and displayed.

### 5. Visualization

- **Plotting Results:** The script visualizes the predicted page views for the next 30 days using both models.

## How to Use

1. Ensure you have Python installed along with the required libraries specified in the script (Pandas, NumPy, Matplotlib, Prophet, NeuralProphet).

2. Place the "wiki_machine_learning.csv" dataset in the same directory as the script.

3. Run the script in a Python environment, considering any specific package dependencies.

## Author

- **Author:** Ilaha Musayeva
- **Date:** 10/20/2023


