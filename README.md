# loan-repayment-clustering
Using a loan dataset, I want to identify which customer groups are more likely to repay loans late using K-Modes clustering algorithm on categorical features. This will help management understand repayment risk and inform lending strategies.

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
