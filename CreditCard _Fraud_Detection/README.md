# Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using machine learning. Fraud detection is a **highly imbalanced problem** where fraudulent transactions are extremely rare (around 0.2% of all transactions). The main goal of this project is to **maximize recall** while detecting fraud, rather than focusing on overall accuracy.

Two approaches were explored:
1. **Classification Models**: Random Forest and XGBoost with oversampling (SMOTE) to handle imbalance.
2. **Anomaly Detection**: Treating fraud transactions as outliers using clustering techniques (optional).

## Dataset
The dataset contains credit card transactions, with numerical features representing anonymized transaction information. The `Class` column indicates whether a transaction is fraud (`1`) or normal (`0`).  

**Download Dataset:** [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

**Class Distribution Example:**
- Normal: 99.8%
- Fraud: 0.2%

## Project Structure
```

credit_card_fraud_detection/
│
├── fraud_eda.ipynb           # Exploratory Data Analysis
├── fraud_model_training.ipynb # Model training with Random Forest and XGBoost
├── fraud_report.docx         # 2-page project report
├── README.md                 # Project overview and instructions

```

## Key Concepts
- **Imbalanced Data Handling:** SMOTE (oversampling minority class) and class weighting.
- **Evaluation Metrics:** Confusion matrix and recall are prioritized; accuracy is not used.
- **Feature Analysis:** EDA includes visualizing class imbalance, transaction amount distribution, and correlation heatmaps.

## How to Run
1. Place `creditcard.csv` in the project folder.
2. Open `fraud_eda.ipynb` to explore the dataset.
3. Open `fraud_model_training.ipynb` to train models and evaluate performance.
4. Check the confusion matrix and classification report to assess model recall.

## Key Learnings
- Imbalanced datasets require special handling; ignoring the minority class leads to misleadingly high accuracy.
- Recall is critical in fraud detection to minimize missed frauds.
- Oversampling and anomaly detection improve the model’s ability to detect rare events.
