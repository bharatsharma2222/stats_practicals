# Practical 6: Statistical Hypothesis Testing Using Teachers' Ratings Dataset

## Objective
To perform different statistical tests on the Teachers' Ratings dataset to analyze the relationship between gender, age, beauty score, teaching evaluation score, and professor rank.

## Dataset
- **Dataset Name:** Teachers' Ratings Dataset (`evalsdataset.csv`)
- **Total Observations:** 463
- **Features Used:** `gender`, `score`, `age`, `bty_avg`, and `rank`
- **Libraries Used:** Pandas and SciPy

## Questions and Implementation

### Q1. T-Test: Does Gender Affect Teaching Evaluation Rates?

- Separated teaching evaluation scores for male and female professors.
- Performed an independent two-sample t-test using `ttest_ind()`.
- Compared the p-value with a significance level of 0.05.

**Hypotheses:**
- **H₀:** Gender does not affect teaching evaluation rates.
- **H₁:** Gender affects teaching evaluation rates.

**Results:**
- T-statistic: 2.7844
- P-value: 0.00558

**Decision:** Reject H₀ because the p-value is less than 0.05.

**Conclusion:** There is a statistically significant difference in teaching evaluation scores between male and female professors.

### Q2. ANOVA: Does Beauty Score Differ by Age?

- Grouped professors according to their age.
- Collected beauty scores (`bty_avg`) for each age group.
- Applied One-Way ANOVA using `f_oneway()`.

**Hypotheses:**
- **H₀:** Beauty score is the same for all age groups.
- **H₁:** Beauty score differs for at least one age group.

**Results:**
- F-statistic: 6.7493
- P-value: 1.2243 × 10⁻²³

**Decision:** Reject H₀ because the p-value is less than 0.05.

**Conclusion:** Beauty scores differ significantly across age groups. ANOVA indicates that at least one age group's mean beauty score is different.

### Q3. Chi-Square Test: Is There an Association Between Tenure and Gender?

- Created a contingency table using `pd.crosstab()`.
- Compared professor rank and gender.
- Applied the Chi-Square test using `chi2_contingency()`.

**Hypotheses:**
- **H₀:** There is no association between tenure/rank and gender.
- **H₁:** There is an
