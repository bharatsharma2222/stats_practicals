Practical 1: Data Handling, Encoding and Matrix Operations Using Titanic Dataset
Objective
To perform data handling, categorical data encoding, conversion of a DataFrame into a NumPy array, and basic matrix operations using Python.

Dataset
Dataset Name: Titanic Dataset (train_titanic.csv)
Total Observations: 891
Total Features: 12
Libraries Used: Pandas and NumPy
Implementation
1. Importing Libraries and Loading Dataset
Imported Pandas and NumPy.
Loaded the Titanic dataset using pd.read_csv().
Displayed the first five rows using head().
2. Exploring the Dataset
Used the following functions:

shape – Displays the number of rows and columns.
columns – Displays all column names.
info() – Displays column data types and non-null values.
Dataset Information:

Rows: 891
Columns: 12
Missing values are present in Age, Cabin, and Embarked columns.
3. Selecting Categorical Data
Selected the categorical columns:

Sex
Embarked
Pclass
Displayed the selected columns using head().

4. One-Hot Encoding
Used pd.get_dummies() to convert categorical values in the Sex and Embarked columns into numerical columns.

New columns created:

Sex_female
Sex_male
Embarked_C
Embarked_Q
Embarked_S
This makes categorical data suitable for numerical operations.

5. Converting DataFrame into NumPy Array
Selected numerical columns using `select_dtypes
