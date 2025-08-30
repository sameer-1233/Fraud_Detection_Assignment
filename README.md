# Fraud Detection Assignment

## 📌 Project Overview
This project focuses on detecting fraudulent transactions using supervised machine learning techniques.  
The dataset (`Fraud.csv`) contains transactional records labeled as fraudulent (`isFraud = 1`) or genuine (`isFraud = 0`).  

The notebook demonstrates:
- Data preprocessing and cleaning
- Handling class imbalance using **SMOTE**
- Building and evaluating fraud detection models
- Extracting insights for fraud prevention

---

## 🛠️ Steps Followed
1. **Data Cleaning**  
   - Checked for missing values (none found).  
   - Handled outliers and checked for multicollinearity.  

2. **Exploratory Data Analysis (EDA)**  
   - Examined fraud vs. non-fraud distribution.  
   - Identified key features influencing fraud (e.g., transaction type, amount, balance differences).  

3. **Train-Test Split**  
   - 80% training, 20% testing with stratified split.  

4. **Class Imbalance Handling**  
   - Applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance fraud cases (~10%).  

5. **Modeling**  
   - **Logistic Regression** (baseline).  
   - **Random Forest Classifier** (final model, strong performance).  

6. **Model Evaluation**  
   - Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC.  
   - **Random Forest achieved ~100% accuracy and ROC-AUC of 0.999**.  

---

## 📊 Key Findings
- Fraudulent transactions are **extremely rare** compared to normal ones.  
- Important predictors: **transaction type, amount, balance differences**.  
- Random Forest outperformed Logistic Regression significantly.  

---

## 📝 Q&A Insights
1. **Data Cleaning:** No missing values, handled imbalance with SMOTE.  
2. **Fraud Detection Model:** Random Forest chosen for its robustness and superior performance.  
3. **Variable Selection:** Included all transaction-related features (type, balances, amounts).  
4. **Performance Tools:** Used confusion matrix, classification report, and ROC-AUC.  
5. **Key Factors:** Type of transaction, amount, and balance discrepancies.  
6. **Do they make sense?** Yes — unusual transactions with large differences are typical fraud indicators.  
7. **Prevention Measures:** Strengthen monitoring, anomaly detection, and real-time flagging.  
8. **Effectiveness Check:** Re-evaluate fraud cases after deployment using KPIs (fraud detection rate, false positives).  

---

## 🚀 How to Run
1. Open the notebook in **Google Colab** or Jupyter.  
2. Upload the `Fraud.csv` dataset.  
3. Run all cells sequentially to reproduce results.  

---

## 📂 Files
- `Fraud_Detection_Assignment.ipynb` → Main notebook with code + results.  
- `Fraud.csv` → Dataset (not included here, but required).  
- `README.md` → Project summary and documentation.  

---

## 👤 Author
**Sameer Pathania**  
Fraud Detection Assignment – August 2025
