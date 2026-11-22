# Decision Tree Classification – Diabetes Dataset

## Overview
This practical implements a Decision Tree Classification model using the Pima Indians Diabetes dataset. The objective is to predict whether a patient has diabetes or not based on different medical features.

## Dataset Information
- **Dataset Name:** Pima Indians Diabetes Dataset
- **Total Observations:** 768
- **Total Features:** 8 independent variables
- **Target Variable:** Outcome
- **Total Columns:** 9

## Features Used
1. Pregnancies
2. Glucose
3. BloodPressure
4. SkinThickness
5. Insulin
6. BMI
7. DiabetesPedigreeFunction
8. Age

**Target Variable:**
- Outcome = 0 (No Diabetes)
- Outcome = 1 (Diabetes)

## Practical Steps

### 1. Data Loading and Exploration (EDA)
- Loaded the diabetes dataset using Pandas.
- Displayed the first five rows using `head()`.
- Checked dataset shape, columns, and data types.
- Generated statistical summary using `describe()`.
- Checked missing values using `isnull().sum()`.

### 2. Feature Selection
- Separated independent variables (X) and dependent variable (y).
- X contains eight independent features.
- y contains the Outcome variable.

### 3. Train-Test Split
- Training data: 80%
- Testing data: 20%
- Used `random_state=42`.
- Applied stratified sampling.

### 4. Decision Tree Classification
- Used `DecisionTreeClassifier` from Scikit-learn.
- Applied Entropy as the splitting criterion.
- Used Information Gain to select the best split.

### 5. Model Prediction and Evaluation
- Predicted outcomes using the test dataset
