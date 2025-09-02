# Credit-Card-Fraud-Detection-
 This project explores the Credit Card Fraud Detection dataset to uncover fraud patterns and detect anomalies. Using EDA, visualization, and outlier detection techniques , we analyzed transaction behaviors and identified key fraud indicators. The study highlights how fraudulent transactions differ in amount, time, and clustering behavior.
#  Credit Card Fraud Detection - Exploratory Data Analysis (EDA)

##  Project Overview
This project explores the **Credit Card Fraud Detection dataset** to analyze **outlier detection** and **fraudulent transaction patterns**.  
Since fraudulent cases are **extremely rare (~0.17%)**, the focus is on **exploratory data analysis (EDA)** and understanding fraud behavior rather than building predictive models.

---

##  Goals
1. Detect unusual transactions (outliers).  
2. Identify fraud patterns across transaction amount, time, and hidden PCA features.  
3. Provide insights & recommendations for **fraud prevention**.  

---

##  Dataset
- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- **Transactions:** 284,807  
- **Features:** 30 anonymized features (PCA transformed), `Amount`, `Time`  
- **Target:** `Class` → `0 = Non-Fraud`, `1 = Fraud`

---

## Exploratory Data Analysis

### 1. Fraud vs Non-Fraud Distribution
- Fraud = **0.17%** of total data → highly imbalanced.  
- Models can get biased toward predicting "Non-Fraud".

### 2. Isolation Forest (Outlier Detection)
- Unsupervised anomaly detection used to flag suspicious cases.  
- Many frauds are captured as outliers.  

### 3. Transaction Amounts
- Fraud transactions often involve **higher amounts**.  
- **Insight:** High-value transactions require stricter monitoring.  

### 4. PCA Visualization
- Fraud cases form **distinct clusters** in 2D PCA space.  
- Helps separate anomalies visually.  

### 5. Time Patterns
- Fraud occurs at **specific times of day**.  
- Suggests possible **coordinated attacks**.  

### 6. Fraud Transactions Over Time
- Clear **fraud spikes** in certain intervals.  
- Fraud is **bursty**, not evenly distributed.  


---

## Key Insights
- Fraud is **rare but distinct** in behavior.  
- Fraudulent transactions are usually **higher in value** and clustered in **time windows**.  
- Outlier detection + visualization helps reveal hidden fraud.  

---

## Conclusion
Fraud detection is challenging due to **data imbalance**, but careful **EDA + anomaly detection** highlights useful fraud indicators.  
A mix of **statistical insights, PCA visualization, and outlier detection** improves understanding of fraud behavior.  

---

## Recommendations
1. Monitor **high-value and unusual-time transactions**.  
2. Deploy **real-time anomaly detection models** (e.g., Isolation Forest).  
3. Balance dataset (SMOTE / undersampling) before training ML models.  
4. Use a **hybrid approach**: unsupervised anomaly detection + supervised ML.  

---

## Skills Used
- **Data Preprocessing:** pandas, numpy  
- **Visualization:** matplotlib, seaborn, plotly  
- **Pattern Recognition:** PCA, time-series analysis  


