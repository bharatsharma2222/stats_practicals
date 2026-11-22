# Practical 5: Probability and Two-Tailed Z-Test Using Python

## Objective
To calculate probabilities using the Teachers' Ratings dataset and perform a two-tailed Z-test using the normal distribution.

## Dataset
- **Dataset Name:** Teachers' Ratings Dataset (`evalsdataset.csv`)
- **Total Observations:** 463
- **Feature Used:** `score`
- **Libraries Used:** Pandas, Math, and SciPy

## Questions and Implementation

### Q1. Probability of Receiving an Evaluation Score Greater Than 4.5

- Selected the `score` column from the dataset.
- Counted the number of evaluation scores greater than 4.5.
- Calculated probability using:

\[
P(X>4.5)=\frac{\text{Number of scores greater than 4.5}}{\text{Total scores}}
\]

**Results:**
- Scores greater than 4.5: 130
- Total scores: 463
- Probability: 0.2808
- Percentage: 28.08%

### Q2. Probability of Receiving an Evaluation Score Between 3.5 and 4.2

- Counted evaluation scores greater than 3.5 and less than 4.2.
- Calculated the probability using:

\[
P(3.5<X<4.2)=\frac{\text{Number of scores between 3.5 and 4.2}}{\text{Total scores}}
\]

**Results:**
- Number of scores: 136
- Total scores: 463
- Probability: 0.2937
- Percentage: 29.37
