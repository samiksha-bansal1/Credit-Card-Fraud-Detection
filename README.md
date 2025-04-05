# 💳 Credit Card Fraud Detection

This project aims to build an effective machine learning pipeline to detect fraudulent credit card transactions. Using real-world anonymized transaction data, we apply preprocessing, class balancing via SMOTE, and classification algorithms (Logistic Regression and XGBoost) to identify fraudulent behavior accurately, especially in the presence of extreme class imbalance.

---

## 📂 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Description**: Transactions made by European cardholders in September 2013.
- **Total Records**: 284,807 transactions
- **Fraud Cases**: 492 (≈ 0.172%)
- **Features**:
  - `V1` to `V28`: PCA-transformed components for anonymity
  - `Time`: Time in seconds from the first transaction
  - `Amount`: Transaction amount
  - `Class`: Target label (`0` = Non-Fraud, `1` = Fraud)

---

## 📊 Project Workflow

### 1. 🧪 Exploratory Data Analysis
- Class imbalance visualization
- Correlation matrix
- Transaction trends over time and amount distribution

### 2. ⚙ Data Preprocessing
- Applied `RobustScaler` to scale `Time` and `Amount` (resilient to outliers)
- Applied **SMOTE** to balance the dataset by oversampling minority class

### 3. 🤖 Modeling
- Models Used:
  - **Logistic Regression**
  - **XGBoost Classifier**
- Model Evaluation Metrics:
  - Confusion Matrix
  - Precision, Recall, F1-score
  - Area Under Precision-Recall Curve (PR AUC)
  - ROC-AUC 

### 4. ✅ Key Results
- Improved recall and F1-score after applying SMOTE
- XGBoost showed better performance on imbalanced data compared to baseline Logistic Regression
- PR AUC highlighted the model’s ability to distinguish fraud despite imbalance

---

## 🚀 Tech Stack

- **Language**: Python  
- **Libraries**:
  - `pandas`, `numpy` – Data manipulation
  - `matplotlib`, `seaborn` – Data visualization
  - `scikit-learn` – ML models and metrics
  - `xgboost` – Advanced boosting model
  - `imbalanced-learn` – SMOTE oversampling

---

## 💻 How to Run the Project

```bash
# 1. Clone the repository
git clone https://github.com/samiksha-bansal1/credit-card-fraud-detection.git

# 2. Navigate into the project directory
cd credit-card-fraud-detection

# 3. Install the dependencies
pip install -r requirements.txt

# 4. Launch the notebook
jupyter notebook Credit_Card_Fraud_Detection.ipynb
