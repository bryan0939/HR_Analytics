# HR Analytics: Predicting Employee Attrition

This project explores machine learning techniques to predict employee attrition using the IBM HR Analytics dataset.

## Objectives

- Understand the key drivers of employee attrition through exploratory data analysis (EDA)
- Preprocess and clean the data for modeling
- Apply and compare Logistic Regression and Random Forest (with SMOTE)
- Evaluate models using precision, recall, F1-score, and ROC AUC
- Interpret the most important features contributing to attrition

## Key Insights

- **OverTime**, **YearsSinceLastPromotion**, and **NumCompaniesWorked** are strong predictors of attrition
- Logistic Regression achieved **recall ~0.70**, making it better suited for identifying at-risk employees
- Random Forest with SMOTE provided a more balanced performance but lower recall

## Model Comparison

| Model                  | Accuracy | Precision | Recall | F1 Score | ROC AUC |
|------------------------|----------|-----------|--------|----------|---------|
| Logistic Regression    | 0.65     | 0.27      | 0.70   | 0.39     | 0.74    |
| Random Forest + SMOTE  | 0.80     | 0.34      | 0.28   | 0.31     | 0.74    |

> **Conclusion**: If your goal is to flag as many potential leavers as possible for HR intervention, Logistic Regression is the better choice.

## Project Structure

```
HR_Analytics_GitHub_Ready.ipynb   # Main notebook with full analysis
README.md                         # Project overview and summary
data/                             # (Optional) Folder for raw CSV files
models/                           # (Optional) Saved model outputs
```

## Dependencies

- Python 3.x
- pandas, numpy, scikit-learn, matplotlib, seaborn
- imbalanced-learn (for SMOTE)



## Dataset

[IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

Created as a university business analytics portfolio project.
