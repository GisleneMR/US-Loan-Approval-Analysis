# US and Canada Loan Approval Analysis

## Overview
This project analyzes a dataset of 50,000 loan applications from the United States and Canada. The goal is to understand how financial behavior, debt levels, and credit history affect loan interest rates, and to predict interest rates using regression models.

## Dataset
The dataset was downloaded from Kaggle:
[Realistic Loan Approval Dataset | US & Canada](https://www.kaggle.com/datasets/parthpatel2130/realistic-loan-approval-dataset-us-canada)

It contains 50,000 rows and 20 columns, including applicant demographics, financial profiles, credit behavior, and loan outcomes based on real US and Canadian banking criteria.

## Project Structure
- `analysis.ipynb` — Jupyter Notebook with the full analysis
- `data.csv` — Original dataset
- `chat.txt` — Documentation of AI chat interactions used during this project

## What This Project Covers
- **Data Cleaning:** Removing identifier columns and checking for duplicates and missing values
- **Exploratory Data Analysis (EDA):** Distribution analysis, outlier detection, and correlation analysis between financial variables
- **Modeling:** Comparison of three regression models — Linear Regression, Polynomial Regression, and Ridge Regression — to predict interest rates
- **Hyperparameter Tuning:** Grid Search to find the best alpha value for Ridge Regression
- **Single vs Multi-Variable Analysis:** Comparing a single-feature model (credit score) against a multi-feature model

## Key Findings
- Credit score is the strongest single predictor of interest rate, but all three models only explained about 24% of the variance (R² ≈ 0.24)
- Polynomial Regression performed slightly better than Linear and Ridge Regression
- The best alpha value for Ridge Regression was 100, though it did not significantly improve performance
- A large portion of interest rate variation likely depends on factors not captured in this dataset, such as lender-specific pricing policies

## Tools Used
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
- Jupyter Notebook
- ChatGPT (OpenAI) for code generation assistance, documented in `chat.txt`

## How to Run
1. Clone this repository
2. Make sure `data.csv` is in the same folder as `analysis.ipynb`
3. Open `analysis.ipynb` in Jupyter Notebook
4. Run all cells from top to bottom
