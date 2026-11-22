# Practical 9 – KNN Classification Using Iris Dataset

## Overview
This practical implements the K-Nearest Neighbors (KNN) classification algorithm using the Iris dataset. The objective is to classify flowers into three species based on their sepal and petal measurements.

## Dataset Information
- **Dataset Name:** Iris Dataset
- **Source:** Scikit-learn built-in dataset
- **Total Observations:** 150
- **Total Features:** 4
- **Target Variable:** Species
- **Number of Classes:** 3

## Features Used
1. Sepal Length (cm)
2. Sepal Width (cm)
3. Petal Length (cm)
4. Petal Width (cm)

## Flower Species
- Setosa
- Versicolor
- Virginica

## Practical Steps

### 1. Import Libraries and Load Dataset
- Imported Pandas, NumPy, Matplotlib and Seaborn.
- Loaded the Iris dataset using Scikit-learn.
- Converted numerical species labels into flower names.

### 2. Exploratory Data Analysis (EDA)
- Displayed the first five rows using `head()`.
- Generated statistical summary using `describe()`.
- Used `groupby()` to count each flower species.
- Checked missing values using `isnull().sum()`.

### 3. Feature Scaling
- Separated independent variables (X) and dependent variable (y).
- Split the dataset into 80% training and
