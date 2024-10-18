# Used Car Price Prediction

This repository provides an end-to-end machine learning pipeline for predicting used car prices. The project leverages advanced techniques in **Exploratory Data Analysis (EDA)**, **feature engineering**, and **model ensembling** to deliver a high-performance predictive model.

## Project Overview
The goal of this project is to predict car prices using various machine learning models, including **CatBoost**, **LightGBM**, and **XGBoost**. These models are combined in an ensemble for robust predictions. Key steps include data preprocessing, feature engineering, hyperparameter optimization, and model evaluation.

## Dataset
The project uses the following datasets:
- [Kaggle Playground Series S4E9](https://www.kaggle.com/competitions/playground-series-s4e9)

Both datasets provide a range of features, such as mileage, engine size, transmission type, and accident history, to help predict the target variable (car price).

## Project Structure
The notebook includes the following components:

### 1. **Exploratory Data Analysis (EDA)**
We start with in-depth EDA to uncover trends and relationships between variables:
- **Fuel Type Distribution**
- **Price vs. Mileage and Model Year**
- **Impact of Accident History on Prices**
- **Price Variations Across Car Brands**

Visualization libraries like `seaborn`, `plotly`, and `matplotlib` are used to create meaningful insights.

### 2. **Feature Engineering**
- Handling missing values
- Creation of categorical and numerical features
- Interaction features between key variables
- Adjusting feature distributions for better model performance

### 3. **Model Training and Evaluation**
Three powerful machine learning models were used:
- **XGBoost**: Gradient boosting algorithm based on decision trees
- **LightGBM**: Gradient boosting framework focused on speed and efficiency
- **CatBoost**: Gradient boosting library for categorical data handling

Each model was trained using **cross-validation** and **hyperparameter tuning**:
- **XGBoost** parameters: `max_depth`, `learning_rate`, `n_estimators`, etc.
- **LightGBM** parameters: `num_leaves`, `learning_rate`, `min_data_in_leaf`, etc.
- **CatBoost** parameters: `learning_rate`, `iterations`, `depth`, etc.

### 4. **Model Ensembling**
To further improve the predictive power, the predictions from the three models were combined using an ensemble technique:
- **Weighted Average Method**: This approach reduces variance and enhances model stability.

### 5. **Hyperparameter Tuning**
Hyperparameter optimization was performed using **Optuna** to find the best configuration for each model. This helped improve the overall accuracy and reduce overfitting.

## Results 🏆
- **Cross-Validation Accuracy**: Each model's performance was evaluated through cross-validation, ensuring robustness across different data splits.
- **Final Ensemble Prediction**: The predictions from each model were combined into a final ensemble, producing high-quality price predictions.



## Conclusion
This project demonstrates the power of **ensemble learning** and **advanced feature engineering** for predicting car prices. By combining multiple models, we were able to achieve robust and accurate predictions.
