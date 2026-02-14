# 📊 Statistics and Machine Learning Exam  
## 🌍 Global Ads Performance Analysis

---

## 📌 Project Overview

This project analyzes global advertising campaign performance using **statistical analysis** and **machine learning techniques**.

The main objectives are to:

- Compare platform ROI  
- Forecast campaign conversions  
- Classify profitable campaigns  
- Discover hidden campaign segments  

---

## 🎯 Problem Statements

### 1️⃣ Platform ROI Comparison  
Test whether **ROAS** differs significantly across:

- TikTok  
- Meta  
- Google  

Using statistical hypothesis testing.

---

### 2️⃣ Conversion Forecasting  
Predict campaign conversions using **supervised machine learning**.

---

### 3️⃣ Profitability Classification  
Classify campaigns as **“Winners” (ROAS > 1)** using pre-revenue indicators.

---

### 4️⃣ Market Segment Discovery  
Identify hidden campaign archetypes using **unsupervised clustering**.

---

## 📂 Dataset Information

- **Source:** Kaggle – Global Ads Performance Dataset  
- **Size:** 500+ observations  
- **Features Include:**  
  - Platform  
  - Industry  
  - Country  
  - Impressions  
  - Clicks  
  - Ad Spend  
  - Revenue  
  - ROAS  
  - And more  
- **Type:** Hybrid  
  - Regression  
  - Classification  
  - Clustering  

---

## 🔄 Project Workflow

### 🧹 Preprocessing

- Handled missing values using:
  - Median imputation  
  - Mode imputation  
- Feature engineering:
  - Month  
  - Week  
  - Day of week  
- Recalculated:
  - CTR  
  - CPC  
  - CPA  
- Outlier clipping (1%–99%)  
- Standardized numerical features  

---

### 🔊 Noise Injection & Cleaning

- Injected **3% Gaussian noise** into financial features  
- Applied **quantile smoothing**  
- Compared:
  - Original data  
  - Noisy data  
  - Cleaned data  

---

### 📊 Statistical Analysis

Calculated:

- Mean  
- Variance  
- Skewness  

Performed:

- **Kruskal–Wallis hypothesis test**

📌 Result:  
Found statistically significant ROAS differences across platforms (**p < 0.05**)

---

## 🤖 Supervised Learning

### 📈 Regression

**Goal:** Predict conversions  

**Models Used:**

- Ridge Regression  
- Random Forest  

**Evaluation Metrics:**

- MAE  
- RMSE  
- R²  

**Result:**  
Random Forest achieved ~93% accuracy.

---

### 🏷️ Classification

**Goal:** Predict profitable campaigns (ROAS > 1)

**Model Used:**

- Random Forest Classifier  

**Evaluation Metrics:**

- F1-score  
- ROC-AUC  

**Result:**  
High AUC even with noisy data.

---

## 🔍 Unsupervised Learning

**Methods Used:**

- PCA (Dimensionality Reduction)  
- K-Means Clustering  

**Cluster Selection:**

- Silhouette Score  
- Optimal k = 3  

**Discovered Campaign Segments:**

- Viral campaigns (high efficiency)  
- Scaled campaigns (high spend)  
- Underperforming campaigns  

---

## 📌 Key Results

- TikTok showed higher agility in certain niches (EdTech, FinTech).  
- The model predicts campaign success with over 90% accuracy.  
- Enables data-driven and automated budget allocation strategies.  

---

## 🚀 Future Work

- Integrate real-time advertising platform APIs  
- Enable live campaign performance forecasting  

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## ▶️ How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone <repository-url>
