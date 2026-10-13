# Advanced Statistical Analysis & Hypothesis Testing

## Project Overview
This project demonstrates statistical analysis and hypothesis testing using Python. It explores a sample dataset and applies statistical methods to assess distributions, compare groups, and examine possible differences between treatment groups.

> **Note:** The dataset used in this project is synthetic and generated for learning purposes. It does not contain real patient data and should not be used to make medical decisions.

## Objectives
- Explore and summarize the dataset.
- Visualize the distribution of recovery days.
- Test whether the data is consistent with a normal distribution.
- Compare two independent groups using parametric and non-parametric tests.
- Compare three treatment groups using One-Way ANOVA and Tukey's HSD.
- Examine the effects of treatment, gender, and their interaction using Two-Way ANOVA.
- Calculate a 95% confidence interval for the difference between two group means.
- Interpret results using a significance level of 0.05.

## Dataset Description
The notebook creates a synthetic dataset with 180 observations and the following columns:

| Column | Description | Type |
|---|---|---|
| `Patient_ID` | Unique identifier for each sample record | Integer / identifier |
| `Age` | Sample age in years | Numerical |
| `Treatment` | Assigned sample group (`Treatment_A`, `Treatment_B`, or `Treatment_C`) | Categorical |
| `Gender` | Sample category (`Male` or `Female`) | Categorical |
| `Recovery_Days` | Simulated number of days to recovery | Numerical |

The values are randomly generated for demonstration and are not intended to represent real-world clinical outcomes.

## Tools and Libraries
- Python 3
- Jupyter Notebook
- pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- statsmodels

## Statistical Methods
1. **Exploratory Data Analysis (EDA):** dataset shape, data types, descriptive statistics, and missing-value checks.
2. **Visualizations:** histogram and box plot of `Recovery_Days`.
3. **Normality testing:** Shapiro–Wilk test and a Kolmogorov–Smirnov-based normality check. Interpret the KS result with care when distribution parameters are estimated from the same sample; a Lilliefors-adjusted test is more appropriate for that setting.
4. **Independent two-sample comparison:** Welch's independent t-test.
5. **Non-parametric comparison:** Mann–Whitney U test.
6. **One-Way ANOVA:** compare mean recovery days across the three treatment groups.
7. **Post-hoc analysis:** Tukey's HSD to investigate pairwise group differences after ANOVA.
8. **Two-Way ANOVA:** evaluate treatment, gender, and the treatment-by-gender interaction.
9. **Confidence interval:** calculate a 95% confidence interval for the mean difference between Treatment A and Treatment B.

## How to Run
1. Install Python and Jupyter Notebook, for example through Anaconda.
2. Open the notebook `Advanced_Statistical_Analysis.ipynb`.
3. Install the required packages by running this cell in the notebook:

   ```python
   %pip install pandas numpy scipy matplotlib seaborn statsmodels
   ```

4. Run the notebook cells from top to bottom.
5. Review the printed test statistics, p-values, plots, confidence interval, and final interpretation.

## Interpreting Results
A common significance level for this project is **α = 0.05**:
- If `p-value < 0.05`, reject the null hypothesis for that test.
- If `p-value >= 0.05`, do not reject the null hypothesis.

A non-significant result does not prove that groups are identical or that the null hypothesis is true. Conclusions should be based on the actual results produced by the notebook, along with the assumptions and limitations of each test.

## Conclusion
This project provides hands-on practice with exploratory data analysis, normality checks, group-comparison tests, ANOVA, post-hoc testing, and confidence intervals. The final conclusion should be written from the notebook's actual outputs rather than assumed in advance. Because the data is synthetic and randomly generated, the findings are for educational demonstration only.

## Project Files
- `Advanced_Statistical_Analysis.ipynb` — notebook containing the analysis, visualizations, test results, and conclusion.
- `README.md` — project overview and instructions.
- `requirements.txt` — optional list of required Python packages.

## Author
Add your name here.
