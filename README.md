# CarPricePrediction

This project is focused on predicting car prices based on various features like fuel type, car age, mileage, and other specifications. The dataset has been preprocessed to make it suitable for machine learning models, including encoding categorical variables and handling missing values.

Project Overview
The goal of this project is to build a machine learning model that can accurately predict the price of a car based on its characteristics. This can be useful for both car buyers and sellers to estimate a fair price based on historical data.

Features
Fuel Type Encoding: Converted the Fuel_Type column from categorical values (Petrol, Diesel, CNG) to numerical values (0, 1, 2), which allows machine learning models to interpret the data more effectively.
Data Cleaning: Removed missing values and handled inconsistencies in the dataset.
Feature Engineering: Created additional features where necessary to improve model performance.
Model Training: Various supervised learning models are tested and compared for performance.
Dataset Description
Fuel_Type: Type of fuel used by the car (e.g., Petrol, Diesel, CNG).
Mileage: The mileage of the car.
Age: Age of the car in years.
Other Features: Additional features like horsepower, transmission type, etc.
Project Structure
Car_Price_Prediction.ipynb: Main Jupyter notebook containing the data preprocessing steps, exploratory data analysis, and model training.
data/: Folder containing the dataset (not provided in this repo for privacy reasons).
models/: Folder for saving trained models.
Data Preprocessing
In order to make the dataset ready for machine learning, the following preprocessing steps were taken:

Encoding Categorical Data:

The Fuel_Type column was encoded with the following mapping:
Petrol → 0
Diesel → 1
CNG → 2
This conversion allows the model to treat fuel types as numerical features, making it easier to interpret during training.
Handling Missing Values: Imputed missing values in specific columns to ensure clean data.

Feature Scaling: Normalized certain features to improve model accuracy and training speed.

Machine Learning Models
The following models were implemented and compared to determine the best performance:

Linear Regression: Simple regression model for baseline comparison.
Decision Trees: Non-linear model that captures interactions between features.
Random Forests: Ensemble method to improve accuracy and reduce overfitting.
Gradient Boosting: Advanced ensemble method for boosting performance on complex data.
Results
Each model was evaluated based on its mean absolute error (MAE), root mean square error (RMSE), and R-squared score. The best-performing model was selected based on these metrics.
