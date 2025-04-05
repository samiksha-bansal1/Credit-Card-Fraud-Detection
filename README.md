---

# 💳 Credit Card Fraud Detection

This project focuses on building a machine learning model to detect fraudulent credit card transactions. It leverages the *Kaggle Credit Card Fraud Detection* dataset and applies data preprocessing, exploratory analysis, SMOTE for class balancing, and classification models to accurately identify fraudulent behavior.

---

## 📂 Dataset

- *Source*: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- *Description*: Transactions by European cardholders in September 2013.
- *Size*: 284,807 transactions
- *Fraudulent Transactions*: 492 (~0.172%)
- *Features*:
  - V1 to V28: PCA-transformed components
  - Time: Time in seconds from the first transaction
  - Amount: Transaction amount
  - Class: Target label (0 = Non-Fraud, 1 = Fraud)

---

## 📊 Workflow

### 1. 📈 Exploratory Data Analysis
- Visualizations of class distribution
- Correlation heatmaps
- Transaction amount and time patterns

### 2. ⚙ Preprocessing
- StandardScaler applied to Amount and Time
- SMOTE used to address *class imbalance* by oversampling the minority class

### 3. 🤖 Modeling
- Models Used:
  - Logistic Regression
  - Random Forest
  - (You can add XGBoost if you used it)
- Model evaluation using:
  - *Confusion Matrix*
  - *Precision, **Recall, **F1-Score*
  - *ROC-AUC*

### 4. 📌 Key Results
- Comparison of performance metrics before and after applying SMOTE
- Discussion of how oversampling affects model behavior and bias

---

## 🚀 Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- *Imbalanced-learn* (for SMOTE)

---

## 📁 How to Run

1. Clone the repository:
   bash
   git clone https://github.com/yourusername/credit-card-fraud-detection.git
   

2. Navigate to the project folder:
   bash
   cd credit-card-fraud-detection
   

3. Install dependencies:
   bash
   pip install -r requirements.txt
   

4. Run the Jupyter Notebook:
   bash
   jupyter notebook Credit_Card_Fraud_Detection.ipynb
   

---

## 🧠 Key Learnings

- Imbalanced data can severely impact model accuracy.
- *SMOTE* can help create a balanced dataset by synthetically oversampling the minority class.
- Evaluation metrics like precision and recall are more appropriate than accuracy in fraud detection.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---
