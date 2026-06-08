# ADHD-Prediction-WiDS-2025
Machine learning models for ADHD diagnosis prediction using the WiDS Datathon 2025 Health Outcomes dataset.
# ADHD Prediction using Machine Learning: WiDS Datathon 2025

## Project Overview
This project develops and evaluates machine learning models for predicting Attention Deficit Hyperactivity Disorder (ADHD) using the WiDS Datathon 2025 Health Outcomes Prediction dataset. The dataset contains socio-demographic variables, behavioural assessments and functional MRI (fMRI) measurements collected from children and adolescents.

## Objective
The objective is to develop predictive models that can support early ADHD identification and provide insights into the factors associated with ADHD diagnosis.

## Dataset
**Source:** WiDS Datathon 2025 Health Outcomes Prediction Dataset

https://www.kaggle.com/competitions/widsdatathon2025

**Target Variable:** ADHD_Outcome

## Data Preprocessing
- Missing value handling using median imputation
- Outlier detection using the IQR method
- Feature scaling using StandardScaler
- Feature selection using SelectKBest (ANOVA F-test)
- 80:20 train-test split with stratification

## Exploratory Data Analysis
- ADHD diagnosis distribution
- Age distribution
- ADHD percentage by age group
- Correlation analysis
- Diagnostic analytics
- Statistical hypothesis testing

## Machine Learning Models
- Logistic Regression
- Random Forest
- Gradient Boosting
- Neural Network (MLP)
- XGBoost

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

## Best Model
XGBoost achieved the best overall performance:

| Metric | Score |
|----------|-------|
| Accuracy | 79.8% |
| Precision | 80.6% |
| Recall | 92.8% |
| F1-score | 86.3% |
| ROC-AUC | 0.821 |

## Model Interpretation
Feature importance analysis identified behavioural variables, particularly SDQ Hyperactivity scores, as the strongest predictors of ADHD. Several fMRI-derived features also contributed to prediction.

## Repository Contents

```
ADHD-Prediction-WiDS-2025
│
├── ADHD_Prediction.ipynb
├── README.md
├── requirements.txt
├── figures/
│      ├── eda_plots.png
│      ├── confusion_matrices.png
│      ├── roc_curves.png
│      └── feature_importance.png
```

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

## Author
MSc Artificial Intelligence and Data Science

## Citation
Women in Data Science (WiDS). (2025). *WiDS Datathon 2025 Health Outcomes Prediction Dataset*. Kaggle.
