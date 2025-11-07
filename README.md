## 🏦 Loan Repayment Clustering: Understanding Borrower Risk

Exploring which customer groups are more likely to repay loans late using unsupervised learning.

## Project Story
Every loan tells a story.
Behind repayment patterns lie human circumstances — income, housing, opportunity.

In this project, I explored how those factors cluster together and what they reveal about loan repayment risk. The goal wasn’t to predict individual defaulters, but to understand which borrower profiles carry more risk, helping lenders make fairer, more informed decisions.

## Objective

*Question: Can we segment borrowers into meaningful groups and identify which groups are most likely to repay loans late?*

This analysis combines data storytelling and unsupervised machine learning to uncover repayment patterns from categorical data.

## Data & Methodology
Dataset is downloaded from this link:
https://www.kaggle.com/datasets/prakashraushan/loan-dataset

1. Data Preparation: handelling mising values, duplicated rows, inconsistant format, encoding categorical features such as *customer_income,loan_intent, loan_grade, interest_rate_bracket, and home_ownership*.
2. Feature Selection:	Chose features correlated with current_loan_status by using *spearman method*.
3. Clustering:	Used K-Modes, a categorical clustering algorithm, to group similar borrowers.
4. Evaluation:	Compared late-repayment percentages across clusters and validated results using a chi-square test.
5. Visualization:	Used bar charts and heatmaps to summarize patterns across groups.

## Key Findings

| Cluster | Customer Profile                                      | % Late Repayment | Interpretation                                                      |
| ------- | ----------------------------------------------------- | ---------------- | ------------------------------------------------------------------- |
| **3**   | Low income (1), Grade C, Very high interest, Rent     | **50.7%**        | 🔴 High risk – financially stretched borrowers with expensive loans |
| **0**   | Mid-high income (4), Grade B, Medium interest, Rent   | 18.5%            | 🟠 Moderate risk – decent income but high living costs              |
| **1**   | Low income (1), Grade A, Low interest, Rent           | 16.2%            | 🟢 Lower risk – safer loans but financially limited                 |
| **2**   | High income (5), Grade A, Very low interest, Mortgage | **8.3%**         | 🟢 Very low risk – stable borrowers with affordable loans           |

*Noted that Grade A is the highest (A>B>C>D>E)*


## Visual Summary
Correlation Matrix

![Correlation Matrix](results/correlation_matrix_spearman.png)

Default Rate by Cluster
![Default Rate](results/Cluster_default_rate_chart.png)

Cluster Feature Profile Heatmap
![Cluster Profile Heatmap](results/cluster_profile_heatmap.png)
The contrast between Cluster 3 and Cluster 2 visually highlights how income, loan terms, and housing status interact to influence repayment reliability.

## Tools
Python, pandas, kmodes, matplotlib, seaborn, Chi-square, numpy
