# Telco Customer Churn Prediction

This project predicts which customers of a telecom company are likely to churn (leave). By analyzing customer data and training machine learning models, the company can take retention actions to reduce churn.

## Folder Structure

```

Customer_Churn/
│
├── telco.csv
│
├── churn_eda.ipynb
│──churn_model_training.ipyn
│
├── churn_report.docx
│ 
── README.md
````

## Dataset
- **Source:** Telco Customer Churn Dataset  
- **Rows:** ~7,000  
- **Columns:** 21  
- **Target:** `Churn` (Yes/No)  

## Models Trained
| Model          | Accuracy | Precision | Recall | F1    | AUC   |
|----------------|---------|-----------|--------|-------|-------|
| Logistic       | 0.804   | 0.648     | 0.572  | 0.608 | 0.836 |
| Decision Tree  | 0.790   | 0.617     | 0.559  | 0.586 | 0.823 |
| Random Forest  | 0.784   | 0.623     | 0.473  | 0.538 | 0.812 |
| XGBoost        | 0.767   | 0.565     | 0.535  | 0.549 | 0.802 |

**Best Model:** Logistic Regression (balanced precision & recall, highest F1 & AUC).

## How to Run
1. Clone this repository:  
   ```bash
   git clone 
````

. Open notebooks in Jupyter or VSCode from the `notebooks/` folder and run the cells.

## Key Insights

* Month-to-month contract customers churn more than 1- or 2-year contract customers.
* Higher monthly charges increase likelihood of churn.
* Logistic Regression provides the best balance between catching churners (recall) and avoiding false positives (precision).
