
# ADHD Prediction using Machine Learning: WiDS Datathon 2025

## Project Overview

This project develops and evaluates machine learning models for predicting Attention Deficit Hyperactivity Disorder (ADHD) using the Women in Data Science (WiDS) Datathon 2025 Health Outcomes Prediction dataset. The dataset contains socio-demographic variables, behavioural assessments, and functional MRI (fMRI) measurements collected from children and adolescents.

## Objective

The objective of this study is to develop predictive models that can support early ADHD identification and provide insights into factors associated with ADHD diagnosis.

## Dataset

**Source:** WiDS Datathon 2025 Health Outcomes Prediction Dataset

https://www.kaggle.com/competitions/widsdatathon2025

**Target Variable:** `ADHD_Outcome`

## Data Preprocessing

* Missing value handling using median imputation
* Outlier detection using the Interquartile Range (IQR) method
* Feature scaling using StandardScaler
* Feature selection using SelectKBest with ANOVA F-test
* Stratified 80:20 train-test split

## Exploratory Data Analysis

* ADHD diagnosis distribution
* Age distribution
* ADHD percentage by age group
* Correlation analysis
* Diagnostic analytics
* Statistical hypothesis testing

## Machine Learning Models

* Logistic Regression
* Random Forest
* Gradient Boosting
* Neural Network (MLP)
* XGBoost

## Evaluation Metrics

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

## Best Model

XGBoost achieved the best overall performance.

| Metric    | Score |
| --------- | ----- |
| Accuracy  | 79.8% |
| Precision | 80.6% |
| Recall    | 92.8% |
| F1-score  | 86.3% |
| ROC-AUC   | 0.821 |

## Model Interpretation

XGBoost feature importance analysis identified behavioural variables, particularly **SDQ Hyperactivity** scores, as the strongest predictors of ADHD. LIME (Local Interpretable Model-Agnostic Explanations) was also used to explain individual predictions and improve model transparency. Several fMRI-derived features contributed to classification performance.

## Repository Structure

```text
ADHD-Prediction-WiDS-2025
│
├── ADHD_Prediction.ipynb
├── README.md
├── requirements.txt
│
├── figures/
│      ├── eda_plots.png
│      ├── confusion_matrices.png
│      ├── roc_curves.png
│      ├── feature_importance.png
│      └── lime_explanation.png
│
├── results/
│      └── model_metrics.csv
```

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Matplotlib
* Seaborn
* LIME

## Installation

Install the required libraries:

```bash
pip install -r requirements.txt
```

## Author

**MSc Data Science Student**
Buckinghamshire New University

## Dataset Citation

Women in Data Science (WiDS). (2025). *WiDS Datathon 2025 Health Outcomes Prediction Dataset*. Kaggle.

https://www.kaggle.com/competitions/widsdatathon2025

## Disclaimer

This project was developed for academic purposes as part of an MSc Data Science programme. The proposed machine learning models are intended to support clinical decision-making and should not be used as standalone diagnostic tools.
