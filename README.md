# Heart Disease Prediction (R) — Data Science Project

## Overview
This project predicts the presence of heart disease using clinical patient attributes.
It follows the **CRISP-DM** methodology and includes **Exploratory Data Analysis (EDA)**,
data preprocessing, model development, and performance evaluation.

## Dataset
- Source: **UCI Heart Disease Dataset (Cleveland)**
- Target variable: `target`
  - `0` = No Heart Disease
  - `1` = Heart Disease

## Workflow (CRISP-DM)
1. **Data Understanding**: EDA (distributions, correlations, outliers, bivariate analysis)
2. **Data Preparation**: missing value handling, one-hot encoding, feature scaling
3. **Modeling**: Logistic Regression, Random Forest, Support Vector Machine (SVM)
4. **Evaluation**: Accuracy, Precision, Recall, F1-score, AUC-ROC, Confusion Matrix
5. **Ethics & Professionalism**: GDPR considerations, bias risks, human-in-the-loop decisions

## Key Visualizations
- Class distribution of the target variable  
- Univariate distributions of clinical features  
- Correlation heatmap  
- Outlier analysis (boxplots)  
- Confusion matrix and ROC curve  

All figures are saved in: `results/figures/`

## Results Summary
Models were compared using multiple metrics. Special attention is given to **false negatives**
(missed disease cases), which is a critical risk in healthcare decision support.

## Tech Stack
- R, tidyverse, ggplot2
- caret (or tidymodels), e1071 (SVM), randomForest
- pROC (AUC/ROC), corrplot or GGally

## How to Run
1. Put `heart.csv` inside `data/`
2. Run scripts in order:
   - `scripts/01_eda.R`
   - `scripts/02_preprocessing.R`
   - `scripts/03_modeling.R`
   - `scripts/04_evaluation.R`

## Author
Sandeep (Ulster University)
