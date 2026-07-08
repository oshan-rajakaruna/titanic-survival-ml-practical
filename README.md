# Titanic Survival Machine Learning Pipeline

## Project Overview

This project is an end-to-end machine learning practical based on the Titanic survival dataset.

The goal of this project is to predict whether a passenger survived or not using passenger information such as passenger class, gender, age, fare, number of family members aboard, and embarkation point.

This project was developed as a practical machine learning workflow to demonstrate data cleaning, exploratory data analysis, feature preprocessing, model training, model evaluation, and result documentation.

---

## Problem Type

This is a **binary classification** problem.

### Target Variable

`Survived`

- `0` = Passenger did not survive
- `1` = Passenger survived

---

## Dataset

The dataset contains passenger-level information from the Titanic.

### Main Columns

- `PassengerId`
- `Survived`
- `Pclass`
- `Name`
- `Sex`
- `Age`
- `SibSp`
- `Parch`
- `Ticket`
- `Fare`
- `Cabin`
- `Embarked`

---

## Project Workflow

The project follows a complete machine learning workflow:

1. Load dataset
2. Check shape, head, and dataset information
3. Identify target column
4. Check missing values
5. Check duplicate records
6. Clean the dataset
7. Perform exploratory data analysis
8. Split features and target
9. Encode categorical variables
10. Split data into training and testing sets
11. Scale feature data
12. Train baseline Logistic Regression model
13. Make predictions
14. Evaluate model performance
15. Explain model results
16. Train and compare Random Forest model
17. Save model outputs and reports
18. Save trained models and scaler
19. Load saved model and test future prediction

---

## Data Cleaning Decisions

The following cleaning decisions were applied:

- Missing `Age` values were filled using the median.
- Missing `Embarked` values were filled using the mode.
- `Cabin` was dropped because it had a high percentage of missing values.
- `PassengerId`, `Name`, and `Ticket` were removed because they were identifiers or high-cardinality text fields not suitable for the basic model.

---

## Exploratory Data Analysis

EDA was performed to understand:

- Survival distribution
- Survival rate by gender
- Survival rate by passenger class
- Age distribution
- Fare distribution
- Numerical summary statistics

EDA helped identify patterns and relationships before model training.

---

## Models Used

Two classification models were trained and compared:

### 1. Logistic Regression

Used as the baseline classification model.

### 2. Random Forest Classifier

Used as a comparison model to capture more complex patterns and analyze feature importance.

---

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Saved Outputs

The following outputs were saved in the `outputs` folder:

- `model_comparison.csv`
- `random_forest_feature_importance.csv`
- `logistic_regression_confusion_matrix.csv`
- `model_accuracy_comparison.png`
- `random_forest_feature_importance.png`

---

## Saved Models

The following files were saved in the `models` folder:

- `logistic_regression_model.pkl`
- `random_forest_model.pkl`
- `standard_scaler.pkl`
- `feature_columns.json`

These files allow the trained model and preprocessing steps to be reused for future predictions.

---

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib
- Jupyter Notebook
- GitHub

---

## Key Learning Outcomes

This project demonstrates:

- How to handle missing values
- How to clean and prepare real-world data
- How to perform EDA
- How to encode categorical variables
- How to split and scale data correctly
- How to train and evaluate classification models
- How to compare models
- How to save trained models and outputs
- How to document a machine learning project professionally

---

## Future Improvements

Possible improvements include:

- Hyperparameter tuning
- Cross-validation
- Advanced feature engineering
- Using pipelines with `ColumnTransformer`
- Testing additional models such as SVM, KNN, or XGBoost
- Creating a simple web app or dashboard for predictions

---

## Project Status

Completed basic end-to-end machine learning workflow.