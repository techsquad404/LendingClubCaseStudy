# Lending Club Case Study

## Introduction
This project focuses on a consumer finance company that specializes in lending various types of loans to urban customers. The main goal is to identify patterns indicating whether a person is likely to default on a loan using Exploratory Data Analysis (EDA).

## Business Understanding
When the company receives a loan application, they must decide whether to approve it based on the applicant’s profile. Two types of risks are associated with this decision:
1. If the applicant is likely to repay the loan, not approving it results in a loss of business.
2. If the applicant is not likely to repay the loan, approving it may lead to financial loss.

By identifying risky loan applicants, the company can reduce credit loss and improve its risk assessment processes.

## Objectives
- Identify the driving factors behind loan defaults.
- Use EDA to understand how consumer attributes and loan attributes influence the tendency of default.
- Provide actionable insights and recommendations based on the analysis.

## Data Understanding
The dataset contains information about past loan applicants and their loan status. Key attributes include:
- Loan Amount
- Funded Amount
- Interest Rate
- Annual Income
- Debt-to-Income Ratio
- Loan Status (Fully Paid, Current, Charged-off)

## Data Cleaning and Manipulation
Data cleaning involved:
- Handling missing values by removing columns with more than 20% missing data and imputing the remaining with mode values.
- Converting percentage columns to numerical values.
- Removing outliers based on z-score analysis.
- Log transformation of skewed numerical columns.

## Exploratory Data Analysis (EDA)
### Univariate Analysis
- Distribution of loan amounts, interest rates, annual incomes, etc.
- Frequency counts of categorical variables like loan status.

### Bivariate Analysis
- Box plots and violin plots for numerical features against loan status to understand the distribution of variables across different loan statuses.
- Scatter plots for numerical features against loan amount to identify correlations and trends.

### Multivariate Analysis
- Correlation matrix to understand relationships between numerical variables.
- Pair plots for a detailed look at interactions between multiple variables.

## Key Findings
- Higher interest rates are associated with higher chances of loan defaults.
- Applicants with lower annual incomes tend to default more frequently.
- Debt-to-Income ratio is a significant predictor of loan defaults.

## Recommendations
- Implement stricter credit checks for applicants with high DTI ratios.
- Adjust interest rates based on the risk profile of the applicant.
- Develop targeted financial products for lower-income applicants to mitigate risk.

## Files in the Repository
- `loan_analysis.ipynb`: Jupyter notebook with detailed analysis and visualizations.
- `Loan Default Prediction Case Study.pdf`: PDF with detailed analysis and explanation.
- `README.md`: This file.

## How to Run
1. Ensure you have Python installed with necessary libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`).
2. Open the Jupyter notebook `loan_analysis.ipynb` for detailed analysis and visualizations.

## Assumptions
- The data provided is representative of the overall loan applicant population.
- Imputed missing values and transformed data accurately reflect the underlying distributions.

## Insights and Summary

### Key Findings
1. **Loan Amount:** Higher loan amounts tend to be associated with higher default rates.
2. **Annual Income:** Lower annual income is correlated with a higher likelihood of default.
3. **Term:** Loans with longer terms are more likely to default.
4. **Employment Length:** Shorter employment lengths are associated with higher default rates.
5. **Credit History:** Applicants with poor credit history (e.g., higher delinquencies, higher revolving utilization) are more likely to default.


## Conclusion
By effectively identifying risky loan applicants, the company can mitigate financial losses and improve its lending strategies, leading to better business outcomes.

## Author
Nandakumar Devadoss and Neeraj Singh
