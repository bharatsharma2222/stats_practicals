# Practical 3 – Teachers' Ratings Dataset Analysis

## Overview
This practical performs data analysis and visualization using the Teachers' Ratings dataset. The objective is to analyse professors' tenure status, ethnicity, age, gender and teaching evaluation scores using Python.

## Dataset Information
- **Dataset Name:** Teachers' Ratings Dataset
- **Total Observations:** 463
- **Total Features:** 23
- **Target Variables:** Age, Gender, Rank, Ethnicity and Score

## Features Used
1. course_id
2. prof_id
3. score
4. rank
5. ethnicity
6. gender
7. language
8. age
9. cls_perc_eval
10. cls_did_eval
11. cls_students
12. cls_level
13. cls_profs
14. cls_credits
15. bty_f1lower
16. bty_f1upper
17. bty_f2upper
18. bty_m1lower
19. bty_m1upper
20. bty_m2upper
21. bty_avg
22. pic_outfit
23. pic_color

## Practical Questions and Steps

### Q1. Percentage of Visible Minority Professors Who Are Tenured
- Filtered professors belonging to visible minorities.
- Calculated the number of tenured minority professors.
- Calculated the percentage of minority professors who are tenured.
- Used a cross-tabulation to compare tenure distribution by ethnicity.

**Result:**
- Total minority professors: 64
- Tenured minority professors: 26
- Percentage: 40.62%

### Q2. Average Age Difference by Tenure
- Created a new column named `Tenure_Status`.
- Grouped professors into Tenured and Untenured categories.
- Calculated mean age and standard deviation for both groups.

**Results:**

| Tenure Status | Mean Age | Standard Deviation |
|---|---:|---:|
| Tenured | 51.89 | 8.65 |
| Untenured | 44.12 | 9.43 |

### Q3. Graph for Age Variable
- Used a histogram to visualize the distribution of professor ages.
- Displayed age on
