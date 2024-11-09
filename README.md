# Car Price Prediction
This project aims to predict car prices based on various features like fuel type, car age, mileage, and other specifications. The dataset has been preprocessed to make it suitable for machine learning models, including encoding categorical variables and handling missing values.

## Project Overview
The goal of this project is to build a machine learning model that can accurately predict the price of a car based on its characteristics. This can be useful for both car buyers and sellers to estimate a fair price based on historical data.

## Features
- **Fuel Type Encoding**: Converted the Fuel_Type column from categorical values (Petrol, Diesel, CNG) to numerical values (0, 1, 2), which allows machine learning models to interpret the data more effectively.
- **Data Cleaning**: Removed missing values and handled inconsistencies in the dataset.
- **Feature Engineering**: Created additional features where necessary to improve model performance.
- **Model Training**: Tested and compared various supervised learning models for performance.

## Dataset Description
The dataset includes the following columns:

- **Fuel_Type**: Type of fuel used by the car (e.g., Petrol, Diesel, CNG).
- **Mileage**: The mileage of the car.
- **Age**: Age of the car in years.
- **Other Features**: Additional features like horsepower, transmission type, etc.

## Project Structure
- `Car_Price_Prediction.ipynb`: Main Jupyter notebook containing the data preprocessing steps, exploratory data analysis, and model training.
- `data/`: Folder containing the dataset (not provided in this repo for privacy reasons).
- `models/`: Folder for saving trained models.

## Data Preprocessing
In order to prepare the dataset for machine learning, the following preprocessing steps were taken:

1. **Encoding Categorical Data**  
   The Fuel_Type column was encoded with the following mapping:  
   - Petrol → 0  
   - Diesel → 1  
   - CNG → 2  
   
   This conversion allows the model to treat fuel types as numerical features, making it easier to interpret during training.

2. **Handling Missing Values**  
   Imputed missing values in specific columns to ensure clean data.

3. **Feature Scaling**  
   Normalized certain features to improve model accuracy and training speed.

## Machine Learning Models
The following models were implemented and compared to determine the best performance:

- **Linear Regression**: A simple regression model for baseline comparison.
- **Decision Trees**: A non-linear model that captures interactions between features.
- **Random Forests**: An ensemble method to improve accuracy and reduce overfitting.
- **Gradient Boosting**: An advanced ensemble method for boosting performance on complex data.

## Results
Each model was evaluated based on the following metrics:

| Model              | Mean Absolute Error (MAE) | Root Mean Square Error (RMSE) | R-squared Score |
|--------------------|---------------------------|-------------------------------|------------------|
| Linear Regression  | e.g., 2300                | e.g., 3000                    | e.g., 0.82      |
| Decision Trees     | e.g., 2100                | e.g., 2800                    | e.g., 0.85      |
| Random Forests     | e.g., 2000                | e.g., 2700                    | e.g., 0.87      |
| Gradient Boosting  | e.g., 1900                | e.g., 2600                    | e.g., 0.88      |

**Note**: Replace the example metric values in the table above with your actual results from the model evaluations.

## Installation
Clone the repository:

```bash
git clone https://github.com/yourusername/Car_Price_Prediction.git
