# Employee Attrition Analysis & Prediction

This project analyzes employee attrition using the IBM HR Analytics dataset and applies machine learning techniques to identify employees at risk of leaving an organization. The objective is to uncover key drivers of attrition and support data-driven HR decisions.

## Objectives
- Analyze factors influencing employee attrition  
- Perform exploratory data analysis (EDA) with business insights  
- Build and compare machine learning models  
- Predict employee attrition and evaluate model performance  

## Dataset
- Source: IBM HR Analytics Employee Attrition Dataset from Kaggle(https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset?select=WA_Fn-UseC_-HR-Employee-Attrition.csv) 
- Records: 1470 employees  
- Target Variable: Attrition (Yes / No)  

## Key Insights
- Sales-related roles show the highest attrition  
- Frequent business travel increases attrition risk  
- Employees working overtime are more likely to leave  
- Lower income and early-career employees have higher attrition  

## Model Performance Comparison

| Metric | Decision Tree | Random Forest |
|------|--------------|---------------|
| Accuracy | 77.8% | **84.8%** |
| Precision (Attrition) | 0.25 | **0.44** |
| Recall (Attrition) | 0.31 | **0.34** |
| F1-score (Attrition) | 0.28 | **0.39** |

Random Forest outperformed the Decision Tree and was selected as the final model due to better generalization and improved detection of attrition cases.

## Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

## Outcome
This project demonstrates how data analysis and machine learning can help HR teams proactively identify employees at risk and reduce attrition.

---

⭐ If you find this project useful, feel free to star the repository!

