
# House Price Prediction

This project aims to predict the sales price of houses using a variety of machine learning models. The dataset used for this project comes from a Kaggle competition, and the evaluation metric is the Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted and the actual sales prices.

## Table of Contents
- [Project Overview](#project-overview)
- [Data](#data)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Ensemble Modeling](#ensemble-modeling)
- [Results](#results)
- [How to Run the Code](#how-to-run-the-code)
- [Resources](#resources)

## Project Overview

The objective of this project is to build a machine learning model that accurately predicts house prices based on various features. The dataset includes detailed information about the houses, such as their size, location, age, and more. The model is trained and evaluated using the Root-Mean-Squared-Error (RMSE) on the logarithm of the house prices to ensure that predictions for both expensive and cheap houses are treated equally.

## Data

The dataset used in this project is from the Kaggle House Prices competition. It contains both training and test datasets with various features related to house properties.

- **Training Data**: Contains the features and the target variable (`SalePrice`).
- **Test Data**: Contains the features only, and the task is to predict `SalePrice` for each entry.

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) was conducted to understand the distribution of variables, detect outliers, and identify any missing data. Key steps included:
- Visualizing distributions of key features.
- Exploring correlations between features and the target variable.
- Identifying and handling missing values.

## Feature Engineering

Feature engineering was performed to enhance the dataset by creating new features and transforming existing ones:
- **New Features**: Additional features were created to capture important aspects like total square footage, age of the house, etc.
- **Transformations**: Logarithmic transformations were applied to skewed features.
- **Encoding**: Categorical features were encoded using techniques such as one-hot encoding.

## Modeling

Several models were developed to predict house prices:
- **Baseline Model**: A simple linear regression model was built as a baseline.
- **Regularized Linear Models**: Ridge and LASSO regressions were used to handle multicollinearity and improve model performance.
- **Advanced Models**: Models like Random Forest, Gradient Boosting Machines (GBM), and XGBoost were implemented to capture non-linear relationships.

## Evaluation

The models were evaluated using cross-validation to ensure robustness and avoid overfitting. The evaluation metric is RMSE on the logarithm of the predicted and actual `SalePrice`. Hyperparameter tuning was performed to optimize model performance.

## Ensemble Modeling

Ensemble techniques were employed to combine the predictions of multiple models to further improve accuracy. This included techniques like stacking and blending, which leverage the strengths of different models.

## Results

The final model achieved competitive results on the test set, demonstrating strong predictive capabilities with minimal overfitting. The ensemble model provided a balanced approach, capturing both linear and non-linear relationships in the data.

## How to Run the Code

1. **Clone the Repository**:
   ```
   git clone https://github.com/umair98392/House_Price_Prediction.git
   cd House_Price_Prediction
   ```
2. **Install Dependencies**:
   Ensure you have the necessary Python packages installed. You can install them using:
   ```
   pip install -r requirements.txt
   ```
3. **Run the Jupyter Notebook**:
   Open the Jupyter notebook and run the cells sequentially to reproduce the analysis and predictions.

4. **Make Predictions**:
   Once the notebook has been executed, predictions on the test set will be generated and can be submitted to Kaggle for evaluation.

## Resources

- [Kaggle Competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)
- [Kaggle Learn](https://www.kaggle.com/learn/overview)
