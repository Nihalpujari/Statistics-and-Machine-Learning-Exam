# Statistics-and-Machine-Learning-Exam
Global Ads Performance Analysis 
Project Overview 
This project analyses global advertising campaign performance using statistical analysis and 
machine learning techniques. 
The goal is to compare platform ROI, forecast conversions, classify profitable campaigns, and 
discover hidden campaign segments. 
Problem Statements 
1. Platform ROI Comparison 
Test whether ROAS differs significantly across TikTok, Meta, and Google using statistical 
hypothesis testing. 
2. Conversion Forecasting 
Predict campaign conversions using supervised machine learning. 
3. Profitability Classification 
Classify campaigns as “Winners” (ROAS > 1) using pre-revenue indicators. 
4. Market Segment Discovery 
Identify hidden campaign archetypes using unsupervised clustering. 
Dataset 
• Source: Kaggle – Global Ads Performance Dataset 
• Size: 500+ observations 
• Features: Platform, Industry, Country, Impressions, Clicks, Ad Spend, Revenue, ROAS, 
and more 
• Type: Hybrid (Regression, Classification, Clustering) 
Project Workflow 
1. Preprocessing 
• Handled missing values using median and mode imputation 
• Feature engineering: 
o Month 
o Week 
o Day of week 
• Recalculated CTR, CPC, and CPA 
• Outlier clipping (1%–99%) 
• Standardized numerical features 
2. Noise Injection & Cleaning 
• Injected 3% Gaussian noise into financial features 
• Applied quantile smoothing 
• Compared original vs. noisy vs. cleaned data 
3. Statistical Analysis 
• Calculated: 
o Mean 
o Variance 
o Skewness 
• Performed Kruskal–Wallis hypothesis test 
• Found significant ROAS differences across platforms (p < 0.05) 
4. Supervised Learning 
Regression 
• Goal: Predict conversions 
• Models: 
o Ridge Regression 
o Random Forest 
• Metrics: 
o MAE 
o RMSE 
o R² 
• Result: 
o Random Forest achieved ~93% accuracy 
Classification 
• Goal: Predict profitable campaigns (ROAS > 1) 
• Model: 
o Random Forest Classifier 
• Metrics: 
o F1-score 
o ROC-AUC 
• Result: 
o High AUC even with noisy data 
5. Unsupervised Learning 
• Method: 
o PCA for dimensionality reduction 
o K-Means clustering 
• Cluster selection: 
o Silhouette score (optimal k = 3) 
• Discovered segments: 
o Viral campaigns (high efficiency) 
o Scaled campaigns (high spend) 
o Underperforming campaigns 
Key Results 
• TikTok showed higher agility in certain niches (EdTech, FinTech) 
• Model predicts campaign success with over 90% accuracy 
• Enables data-driven and automated budget allocation strategies 
Future Work 
• Integrate real-time advertising platform APIs 
• Enable live campaign performance forecasting 
Technologies Used 
• Python 
• Pandas 
• NumPy 
• Scikit-learn 
• Matplotlib / Seaborn 
How to Run the Project 
1. Clone the repository: 
2. git clone <your-repo-link> 
3. Install dependencies: 
4. pip install -r requirements.txt 
5. Open the notebook: 
6. jupyter notebook 
7. Run the main notebook. 
Authors 
• Namrata Bhoyar 
• Nihal Pujari 
• Anuj Kamble 
• Gourav Somanna 
• Pramodkumar Shivanna
