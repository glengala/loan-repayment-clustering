## 🏦 Loan Repayment Clustering: Understanding Borrower Risk

Exploring which customer groups are more likely to repay loans late using unsupervised learning.

## Project Story
Every loan tells a story.
Behind repayment patterns lie human circumstances — income, housing, opportunity.

In this project, I explored how those factors cluster together and what they reveal about loan repayment risk. The goal wasn’t to predict individual defaulters, but to understand which borrower profiles carry more risk, helping lenders make fairer, more informed decisions.

## Objective

*Question: Can we segment borrowers into meaningful groups and identify which groups are most likely to repay loans late?*

This analysis combines data storytelling and unsupervised machine learning to uncover repayment patterns from categorical data.

## Data
Dataset is downloaded from this link:
https://www.kaggle.com/datasets/prakashraushan/loan-dataset

## Steps
1. Preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature selection
4. Clustering (K-Modes)
5. Cluster profiling
6. Repayment behaviour analysis

## Key Findings
- Cluster 3 (low-income renters, high-rate loans with Grade C loan) shows 50% late repayment.
- Cluster 2 (high-income homeowners, low-rate loans with Grade A loan) shows 8% late repayment.
- Noted that Grade A is the highest (A>B>C>D>E)

## Tools
Python, pandas, kmodes, matplotlib, seaborn, Chi-square, numpy
