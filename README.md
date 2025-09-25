# fraud-guard

**fraud-guard** is a machine learning project focused on detecting fraudulent credit card transactions.  
Using classification models and techniques to handle imbalanced data, it demonstrates how ML can be applied to real-world financial problems where accuracy alone is not enough.  

---

## Why This Project?
Credit card fraud is rare but extremely costly. In datasets where fraudulent cases make up less than 0.2% of transactions, traditional models fail by simply predicting "legit" every time.  
This project shows how to:
- **Balance imbalanced data** with undersampling.  
- **Train multiple models** (Logistic Regression, Random Forest, XGBoost).  
- **Evaluate beyond accuracy** with metrics like Recall, Precision, F1, ROC-AUC.  
- **Visualize fraud detection performance** through confusion matrices and ROC curves.  

---

## Project Workflow
1. **Data Exploration** – Inspect dataset, verify imbalance, visualize class distribution.  
2. **Preprocessing** – Scale `Time` and `Amount` using `StandardScaler`, apply undersampling on training data.  
3. **Model Training** – Logistic Regression, Random Forest, XGBoost.  
4. **Evaluation** – Compare models using key metrics on the *original imbalanced* test set.  
5. **Results & Insights** – Highlight trade-offs between Recall and Precision.  

---

## Results
| Model                | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression   | 96.03%   | 3.8%      | 91.8%  | 7.3%     | 0.9760  |
| Random Forest         | 96.41%   | 4.2%      | 91.8%  | 8.0%     | 0.9777  |
| XGBoost               | 95.41%   | 3.3%      | 91.8%  | 6.4%     | 0.9749  |

**Key Insight:**  
- All models achieved **high recall (~92%)**, catching most fraud.  
- Precision was low (~3–4%), meaning more false positives – a trade-off that is often acceptable in fraud detection.  
- **Random Forest** offered the best overall balance with the highest ROC-AUC.  

---

## Future Improvements
- Hyperparameter tuning (GridSearchCV / RandomizedSearchCV).  
- Advanced resampling (SMOTE, ADASYN).  
- Cost-sensitive learning to penalize missed fraud cases more heavily.  
- Feature engineering with domain knowledge.  
- Anomaly detection models tailored for skewed data.  

---

## Tech Stack
- **Python**: pandas, numpy, matplotlib, seaborn  
- **ML**: scikit-learn, imbalanced-learn, XGBoost  
- **Notebook**: Jupyter  

---

## Run Locally
```bash
git clone https://github.com/saadhtiwana/fraud-guard.git
cd fraud-guard
jupyter notebook Credit_Card_Fraud_Detection_Saad.ipynb
````

---

## Author

**Malik Saad Hayat**
[github.com/saadhtiwana](https://github.com/saadhtiwana)

```

