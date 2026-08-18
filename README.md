# Fraud Detection & Transaction Risk Analysis

A machine-learning project focused on identifying potentially fraudulent transactions and converting model predictions into practical transaction-risk decisions.

## Project Overview

Financial fraud detection is a classification problem where the goal is to identify suspicious transactions while minimizing unnecessary false alarms.

This project develops an end-to-end fraud detection workflow covering:

- Exploratory Data Analysis (EDA)
- Transaction pattern analysis
- Data preprocessing
- Feature engineering
- Machine learning classification
- Model evaluation
- Feature importance
- Risk classification
- Interactive risk dashboard

The project compares **Logistic Regression** and **Random Forest** to evaluate their ability to distinguish fraudulent transactions from legitimate transactions.

---

## Research Question

> **Can machine-learning models effectively identify fraudulent transactions while maintaining a practical balance between detecting fraud and minimizing false alerts?**

---

## Objectives

The project aims to:

1. Understand the structure and characteristics of transaction data.
2. Identify patterns associated with fraudulent transactions.
3. Prepare the dataset for machine-learning modelling.
4. Engineer relevant features for fraud detection.
5. Compare Logistic Regression and Random Forest.
6. Evaluate models using fraud-detection-focused metrics.
7. Identify the features most associated with fraud predictions.
8. Convert model predictions into practical transaction-risk categories.

---

## Analytical Workflow

The project follows the workflow:

**Raw Transaction Data → Data Cleaning → EDA → Feature Engineering → Model Training → Model Evaluation → Risk Classification → Dashboard**

---

## Exploratory Data Analysis

The analysis investigates:

- Transaction distributions
- Fraud vs legitimate transaction frequency
- Transaction types
- Transaction amounts
- Account-related characteristics
- Patterns in suspicious transactions
- Relationships between relevant variables

EDA is used to understand the dataset before applying machine-learning models.

---

## Feature Engineering

Relevant transaction and account-level variables are prepared for modelling.

Feature engineering focuses on transforming the available transaction information into variables that can help models distinguish between legitimate and potentially fraudulent activity.

The exact features used are documented in the analysis files.

---

## Machine Learning Models

### Logistic Regression

Logistic Regression provides an interpretable baseline classification model.

It estimates the probability that a transaction belongs to the fraudulent class.

### Random Forest

Random Forest is used as a non-linear ensemble model capable of capturing more complex relationships between transaction features.

The two models are compared using the same evaluation framework.

---

## Model Evaluation

Because fraud datasets can be highly imbalanced, accuracy alone is not sufficient to evaluate model performance.

The project evaluates models using:

| Metric | Purpose |
|---|---|
| Precision | Measures how many transactions predicted as fraud were actually fraudulent |
| Recall | Measures how many actual fraudulent transactions were detected |
| F1-Score | Balances precision and recall |
| ROC-AUC | Measures the model's ability to distinguish between classes |

### Why Recall Matters

Missing a fraudulent transaction can be costly.

Therefore, fraud detection requires careful consideration of the trade-off between:

**Fraud Detection → False Alerts → Operational Cost**

A model with high accuracy but poor fraud recall may not be practically useful.

---

## Risk Decisioning

The project extends beyond a simple fraud/not-fraud prediction.

Model outputs are translated into three practical risk categories:

| Risk Level | Interpretation |
|---|---|
| **Low Risk** | Transaction appears consistent with legitimate activity |
| **Review** | Transaction shows characteristics requiring additional verification |
| **High Risk** | Transaction has a high estimated probability of fraudulent activity |

This framework demonstrates how machine-learning predictions can support operational decision-making.

---

## Feature Importance

Feature importance is examined to understand which variables contribute most strongly to the Random Forest model's predictions.

This improves interpretability and helps identify transaction characteristics associated with elevated fraud risk.

> Model predictions should be interpreted as risk signals rather than proof that a transaction is fraudulent.

---

## Project Outputs

The project produces:

- Exploratory data analysis
- Fraud-pattern analysis
- Feature-engineered dataset
- Logistic Regression model
- Random Forest model
- Model comparison
- Precision / Recall / F1 / ROC-AUC evaluation
- Feature importance analysis
- Risk classification framework
- Interactive fraud-risk dashboard

---

## Dashboard

The project includes an interactive dashboard designed to translate model outputs into a practical transaction-risk monitoring interface.

The dashboard focuses on:

- Transaction monitoring
- Fraud indicators
- Risk classification
- Model insights
- Decision-support information

---

## Tools & Technologies

**Programming & Analysis**

- Python
- Pandas
- NumPy

**Machine Learning**

- Scikit-learn
- Logistic Regression
- Random Forest

**Visualization**

- Matplotlib
- Data Visualization
- Interactive Dashboard

**Development**

- Jupyter Notebook
- GitHub

---

## Project Structure

```text
fraud-detection-transaction-risk/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── fraud_detection_analysis.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   └── models.py
│
├── models/
│   └── model_results/
│
├── visuals/
│   ├── eda/
│   ├── model_evaluation/
│   └── feature_importance/
│
└── dashboard/
    └── fraud-risk-dashboard

## Key Takeaways

The project demonstrates an end-to-end approach to fraud analytics:

**Data → Patterns → Features → Models → Evaluation → Risk Decisions**

The key focus is not simply achieving high predictive accuracy, but understanding the trade-off between **fraud detection and false alerts** and translating machine-learning outputs into practical risk decisions.

---

## Limitations

Several limitations should be considered:

- Historical transaction data may not fully represent current fraud patterns.
- Fraud datasets can contain substantial class imbalance.
- Model performance depends on the quality and representativeness of the available data.
- False positives can create operational costs.
- Fraud patterns can change over time.
- Model predictions should be validated before being used in real-world financial systems.

---

## Future Improvements

Potential extensions include:

- Hyperparameter optimization
- Cross-validation
- Class-imbalance techniques
- Threshold optimization
- Time-based validation
- Explainable AI techniques
- Model monitoring
- Real-time fraud scoring
- Operational-cost modelling
- Advanced ensemble models

---

## Author

**Tanmay Gupta**

B.Tech Computer Science Engineering  
LJ University, Ahmedabad

**Email:** guptatanmay2806@gmail.com

**Portfolio:** [Add your portfolio URL]

**LinkedIn:** [Add your LinkedIn URL]

**GitHub:** [Guptatanmay28](https://github.com/Guptatanmay28)

---

## Disclaimer

This project is intended for **academic, educational and portfolio purposes**.

The models and risk classifications presented in this repository are not intended to replace professional fraud investigation systems or financial-institution risk controls.
