# Credit Card Fraud Detection

This project analyzes a dataset of credit card transactions to detect fraudulent activity using machine learning. The primary goal is to build a classification model that can effectively identify fraudulent transactions in highly imbalanced data.

---

## Dataset Overview

- **Source**: [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- The dataset contains **284,807** transactions with **30 features**, where:
  - Most features are anonymized (V1–V28) due to confidentiality.
  - `Time` and `Amount` are original features.
  - The `Class` column is the target:
    - `0` = legitimate transaction
    - `1` = fraudulent transaction

---

## Tools & Libraries Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- StandardScaler (data normalization)
- RandomForestClassifier (model training)

---

## ⚙️ Process

1. **Exploratory Data Analysis**
   - Visualized class imbalance
   - Summary statistics

2. **Data Preprocessing**
   - Standardized `Time` and `Amount` features
   - Addressed severe class imbalance via *undersampling*

3. **Model Training**
   - Trained a **Random Forest Classifier**
   - Evaluated using accuracy, precision, recall, F1-score

4. **Model Evaluation**
   - Focused on performance metrics suitable for imbalanced classification problems
   - Insights provided into model limitations and next steps

---

## Results

- The model was able to detect fraudulent activity with a strong balance between recall and precision (especially important in fraud detection).
- Undersampling helped address imbalance but at the cost of using fewer data points.
- Future improvements may include:
  - Trying **SMOTE** for oversampling
  - Exploring other classifiers like **XGBoost** or **Logistic Regression**

---

## What I Learned

- Handling imbalanced datasets is crucial in real-world machine learning.
- Random Forest is robust but should be tuned with care.
- Preprocessing and clear evaluation make or break fraud models.

---

## Sample Visualization

![Class Distribution](images/class_distribution.png)

> *Class imbalance is a critical issue — only ~0.17% of transactions are fraudulent.*

---

## How to Run This Project

1. Clone the repo
2. Open the `credit_card_fraud_detection.ipynb` notebook
3. Run cells in order (Google Colab or Jupyter Notebook)

---

## Author

**Naomi Berumen**  
*Aspiring Data Analyst | AI Enthusiast | Always Learning*


---
