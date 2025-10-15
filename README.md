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


**Key Insight:**

* High recall (~92%) ensures most fraud is caught
* Low precision (~3–4%) leads to false positives, acceptable in this domain
* Random Forest achieves the best overall balance


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


