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
<img width="973" height="577" alt="image" src="https://github.com/user-attachments/assets/a39ec92b-3826-4e78-acf5-8b48d2fe1101" />

- Univariate distributions of clinical features
<img width="597" height="840" alt="image" src="https://github.com/user-attachments/assets/3b1f7594-abe0-447b-870e-151e368d04b3" />
- Correlation heatmap
 <img width="555" height="835" alt="image" src="https://github.com/user-attachments/assets/c8d68770-a0db-460a-9db8-d8eb3a8ab63e" /> 
- Outlier analysis (boxplots)
 <img width="541" height="988" alt="image" src="https://github.com/user-attachments/assets/cd039509-f5cb-47b6-b760-da16511b0b33" />  
- Confusion matrix and ROC curve  

<img width="523" height="357" alt="image" src="https://github.com/user-attachments/assets/3f608797-c651-4fd4-9f43-86dde8e9ded3" />


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
