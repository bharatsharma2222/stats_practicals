# Practical 4: Data Analysis and Visualization Using Teaching Ratings Dataset

## Objective
To analyze the Teaching Ratings dataset using Python and perform data analysis and visualization to understand professor details, teaching evaluation scores, age, gender, and tenure status.

## Dataset
- **Dataset Name:** Teaching Ratings Dataset (`evalsdataset.csv`)
- **Total Observations:** 463
- **Total Features:** 23
- **Library Used:** Pandas and Matplotlib

## Questions and Implementation

### Q1. Identify Duplicate Cases Using `prof_id`

- Identified duplicate records using the `prof_id` column.
- Calculated the average age and standard deviation before filtering.
- Removed duplicate professor records to keep one observation per instructor.
- Calculated the average age and standard deviation after filtering.

**Results:**

| Measurement | Before Filtering | After Filtering |
|---|---:|---:|
| Total observations | 463 | 94 |
| Average age | 48.37 | 47.23 |
| Standard deviation | 9.80 | 10.27 |

### Q2. Bar Chart: Lower-Division Courses and Evaluation

- Counted the number of lower-division and upper-division courses.
- Calculated the average teaching evaluation score for each course level.
- Created a bar chart to compare the average evaluation scores.

**Course Distribution:**
- Upper-level courses: 306
- Lower-level courses: 157

**Conclusion:** The bar chart helps compare the average teaching evaluation scores of lower-division and upper-division courses. The higher bar represents the course level with the higher average evaluation.

### Q3. Relationship Between Age and Teaching Evaluation

- Created a scatter plot using age and teaching evaluation score.
- Used age on the X-axis and teaching evaluation score on the Y-axis.
- Observed the relationship between professors' age and their teaching evaluation scores.

### Q4. Age and Teaching Evaluation by Gender

- Created gender-differentiated scatter plots.
- Used different labels for male and female professors.
- Compared teaching evaluation scores across different age groups and genders.

### Q5. Age and Evaluation Scores by Gender and Tenure/Rank

- Created a scatter plot differentiated by gender and professor rank.
- Used the `gender` and `rank` columns to categorize the data.
- Professor ranks included:
  - Tenure track
  - Tenured
  - Teaching

**Conclusion:** The scatter plot shows the relationship between professors' age and teaching evaluation scores, differentiated by gender and rank. Evaluation scores are spread across different age groups, indicating that age alone does not determine teaching evaluation scores. Different genders and ranks show variation in scores, while many professors receive relatively high evaluations (around 4.0–5.0).

## Libraries Used

- **Pandas:** For loading, filtering, and analyzing dataset records.
- **Mat
