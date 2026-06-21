# A/B Test Analysis: E-Commerce Conversion Rate

## Overview
This project analyzes the results of an A/B test conducted by an e-commerce 
company to determine whether a newly designed web page leads to higher user 
conversion rates than the existing page.

## Key Questions
- Does the new page lead to statistically significantly higher conversion rates?
- Does a user's country influence whether they convert?
- Is there an interaction between country and page type on conversion?

## Methods
- Descriptive statistics and exploratory data analysis
- Probability analysis by group and country
- Simulation-based hypothesis testing (500 iterations)
- Logistic regression using statsmodels

## Key Findings
- The treatment page converted at **15.5%** vs **10.5%** for the control page
- The difference is statistically significant (p-value = 0.0)
- Country does not significantly impact conversion rates (US p=0.170, UK p=0.905)
- **Recommendation:** Strong statistical evidence supports implementing the new page

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Jupyter Notebook

## Dataset
The dataset contains 69,889 user sessions with the following columns:
- `country` — User's country (US, UK, CA)
- `group` — Control or treatment group
- `converted` — Whether the user converted (1) or not (0)
