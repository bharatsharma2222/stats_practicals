# TeachingRatings Dataset Analysis

## Aim
To perform Exploratory Data Analysis (EDA) and statistical analysis on the TeachingRatings dataset using Python. The practical focuses on descriptive statistics, data visualisation, and hypothesis testing.

## Dataset
The dataset used is `evalsdataset.csv`.

It contains information about professors and their teaching evaluations, including:
- Professor ID
- Course ID
- Teaching evaluation score
- Gender
- Age
- Rank
- Number of students
- Beauty ratings
- Course details

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Google Colab

## Questions and Analysis

### Q1. Identify the type of data
The dataset is **cross-sectional data** because it contains information about different professors and courses at a particular point or period, rather than tracking the same subjects over time.

### Q2. Calculate mean, median, minimum, and maximum number of students
The `cls_students` column was used to calculate descriptive values.

| Statistic | Result |
|---|---:|
| Mean | 55.18 |
| Median | 29 |
| Minimum | 8 |
| Maximum | 581 |

**Conclusion:** The average class size is approximately 55 students. The median is 29, which indicates that some larger classes increase the mean.

### Q3. Perform descriptive statistical analysis
The `describe()` function was used to calculate count, mean, standard deviation, minimum, maximum, and quartiles for numerical columns.

**Conclusion:** Descriptive statistics help us understand the distribution, central tendency, and variation of the dataset.

### Q4. Plot a histogram of the beauty variable
A histogram was created using the `bty_avg` column to understand the distribution of professors' average beauty scores.

**Conclusion:** The histogram shows that beauty scores are concentrated around the middle values, with a slight positive (right) skew.

### Q5. Compare beauty scores by gender
The mean and standard deviation of beauty scores were calculated separately for male and female professors. Duplicate professor records were removed so that each professor was counted once.

| Gender | Count | Mean | Standard Deviation |
|---|---:|---:|---:|
| Female | 40 | 4.925 | 1.622 |
| Male | 54 | 4.358 | 1.545 |

An independent two-sample t-test was performed.

- **T-statistic:** -1.722
- **P-value:** 0.0884

**Conclusion:** Female professors have a higher average beauty score in this dataset. However, the p-value is greater than 0.05, so the difference is not statistically significant at the 5% significance level.

### Q6. Analyse the relationship between gender and tenure
The percentage of tenured and non-tenured professors was calculated for each gender.

| Gender | Not Tenured | Tenured |
|---|---:|---:|
| Female | 55.00% | 45.00% |
| Male | 33.33% | 66.67% |

A Chi-square test of independence was performed.

- **Chi-square statistic:** 3.571
- **P-value:** 0.0588
- **Degrees of freedom:** 1

**Conclusion:** The percentage of tenured male professors is higher than that of female professors in this dataset. However, the p-value is greater than 0.05, so there is no statistically significant association between gender and tenure status at the 5% significance level.

## Important Note
The dataset contains multiple course records for some professors.

- For Q2 and Q3, all 463 rows were used.
- For Q4, Q5, and Q6, duplicate professor records were removed, leaving 94 unique professors.

This ensures that professor-level comparisons do not count the same professor multiple times.

## Overall Conclusion
In this practical, we analysed the TeachingRatings dataset using Python. We performed descriptive statistical analysis, created a histogram, compared beauty scores by gender using an independent t-test, and examined the relationship between gender and tenure using a Chi-square test.

The analysis showed that female professors had a higher average beauty score, while male professors had a higher percentage of tenured positions. However, neither difference was statistically significant at the 5% significance level.

## Learning Outcomes
- Learned to load and explore a CSV dataset using Pandas.
- Understood cross-sectional data.
- Applied descriptive statistical methods.
- Created histograms using Matplotlib.
- Performed an independent two-sample t-test.
- Performed a Chi-square test of independence.
- Learned how to interpret p-values and statistical test results.
