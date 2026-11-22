 Practical 7 – Statistical Analysis of Teaching Ratings Dataset

Overview
This practical performs statistical analysis on the TeachingRatings dataset to understand the relationship between gender, age, beauty score, and teaching evaluation ratings.

 Dataset
- **Dataset Name:** TeachingRatings
- **Total Observations:** 463
- **Total Features:** 12
- **Source:** TeachingRatings dataset (AER)

Questions Covered

Q1. Regression with T-test
**Question:** Does gender affect teaching evaluation rates?

- Method: Linear Regression (OLS)
- Independent Variable: Gender (female)
- Dependent Variable: Teaching Evaluation (eval)

 Q2. Regression with ANOVA
**Question:** Does the beauty score of instructors differ by age?

- Method: ANOVA
- Independent Variable: Age Group
- Dependent Variable: Beauty Score

 Q3. Correlation / Regression
**Question:** Is teaching evaluation score correlated with beauty score?

- Method: Linear Regression (OLS)
- Independent Variable: Beauty Score
- Dependent Variable: Teaching Evaluation (eval)

Technologies Used
- Python
- Pandas
- NumPy
- Statsmodels
- SciPy
- Jupyter Notebook / Google Colab

Installation

Install the required libraries:

```bash
pip install pandas numpy statsmodels scipy
```

## How to Run
1. Clone or download this repository.
2. Open the Jupyter Notebook.
3. Install the required libraries.
4. Run all cells to see the statistical analysis results.

## Conclusion
This practical uses statistical methods to analyse how gender and beauty scores relate to teaching evaluation ratings and whether instructor beauty scores differ across age groups.
