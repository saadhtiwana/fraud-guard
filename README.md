# Fraud-Guard

**Fraud-Guard** is a machine learning project for detecting fraudulent credit card transactions. It demonstrates how ML can tackle **real-world problems** where accuracy alone isn’t enough.

---

## Why This Project

Credit card fraud is rare (<0.2% of transactions) but costly. Standard models fail by predicting “legit” almost all the time.

Fraud-Guard focuses on:

* Handling imbalanced datasets with **undersampling**
* Training multiple models (Logistic Regression, Random Forest, XGBoost)
* Evaluating models with metrics that matter: **Recall, Precision, F1, ROC-AUC**
* Visualizing results to understand model performance

---

## Project Workflow

1. **Data Exploration** – Check dataset, visualize class imbalance
2. **Preprocessing** – Scale `Time` and `Amount`, undersample training data
3. **Model Training** – Logistic Regression, Random Forest, XGBoost
4. **Evaluation** – Confusion matrices, ROC curves, detailed metrics
5. **Insights** – Trade-offs between Recall and Precision

---

## Results

| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Logistic Regression | 96.03%   | 3.8%      | 91.8%  | 7.3%     | 0.9760  |
| Random Forest       | 96.41%   | 4.2%      | 91.8%  | 8.0%     | 0.9777  |
| XGBoost             | 95.41%   | 3.3%      | 91.8%  | 6.4%     | 0.9749  |

**Key Insight:**

* High recall (~92%) ensures most fraud is caught
* Low precision (~3–4%) leads to false positives, acceptable in this domain
* Random Forest achieves the best overall balance

---

## Future Improvements

* Hyperparameter tuning (GridSearchCV / RandomizedSearchCV)
* Advanced resampling techniques (SMOTE, ADASYN)
* Cost-sensitive learning
* Feature engineering with domain knowledge
* Explore anomaly detection models

---

## Tech Stack

* **Python**: pandas, numpy, matplotlib, seaborn
* **ML**: scikit-learn, imbalanced-learn, XGBoost
* **Notebook**: Jupyter

---

## Run Locally

```bash
git clone https://github.com/saadhtiwana/fraud-guard.git
cd fraud-guard
jupyter notebook Credit_Card_Fraud_Detection_Saad.ipynb
```

---

## Author

**Malik Saad Hayat**
[GitHub: saadhtiwana](https://github.com/saadhtiwana)


