# README for Fraud Detection and Claim Prediction Notebook

# Overview
This notebook is designed to analyze insurance claim data for both fraud detection and claim amount prediction. 
It applies various data analysis techniques, machine learning models for regression and classification, and uses data balancing methods such as SMOTE.

# Data Loading and Preliminary Analysis
* Data Loading and Inspection: Initial data loading to explore structure and basic statistics, including missing values and data types.

# EDA
* Statistical Summary: Descriptive statistics for numerical features and visualization of distributions.
* Univariate and Bivariate Analysis
* Categorical and Numerical Analysis: Distribution analysis using histograms, count plots, and pie charts for categorical variables.
* Relationship Analysis: Exploring relationships between categorical variables and the 'fraud_reported' status through visual analytics.

# Correlation and Cluster Analysis
* Correlation Matrix: Analyzing inter-feature correlations and their impact on fraud reporting.
* Cluster Analysis: Segmenting data into clusters using the Elbow Method and K-means clustering to identify intrinsic groupings within the data.

# Models
**Regression Model for Claim Prediction**
* Data Preparation: Preprocessing steps including handling of multicollinearity and data normalization.
* Model Building and Metrics: Construction of a regression model to predict claim amounts, evaluated using accuracy, R-squared, or similar metrics.
* 
***Total claim amount: 61500, Predicted claim amount: 63867.52952431159***
***Total claim amount: 64350, Predicted claim amount: 64843.336766271415***
***Total claim amount: 81800, Predicted claim amount: 68945.39390584466***
***Total claim amount: 5100, Predicted claim amount: 8126.21607554318***
***Total claim amount: 76120, Predicted claim amount: 65327.77771332724***
***Total claim amount: 53800, Predicted claim amount: 59954.66135142447***
***Total claim amount: 51810, Predicted claim amount: 57961.90250807958***
***Total claim amount: 59520, Predicted claim amount: 61608.13272941043***
***Total claim amount: 32670, Predicted claim amount: 51343.376030701475***
***Total claim amount: 104610, Predicted claim amount: 77325.5709994929***

**Classification Model for Fraud Detection**
* SMOTE Analysis: Application of Synthetic Minority Over-sampling Technique (SMOTE) to address class imbalance in the dataset, enhancing the model’s ability to detect fraud.
* Model Training and Evaluation: A classification model is trained to detect fraudulent claims, with performance metrics such as accuracy and F1-score discussed.

***Metrics     precision    recall  f1-score   support***
      ***N         0.75      0.99      0.86       151***
      ***Y         0.00      0.00      0.00        49***
***accuracy                            0.75       200***
***macro avg       0.38      0.50      0.43       200***
***weighted avg    0.57      0.75      0.65       200***

**WITHOUT SMOTE**

**WITH SMOTE**

**Model    	              Accuracy	AUC	Recall	Prec.	F1	Kappa	MCC***
***SVM - Linear Kernel	0.7967	0	0.7967	0.7901	0.7563	0.2962	0.3590**

***Metrics       precision    recall  f1-score   support***
***Not Fraud        0.80      0.97      0.88       226***
***Fraud            0.76      0.26      0.38        74***
***accuracy                             0.80       300***
***macro avg        0.78      0.62      0.63       300***
***weighted avg     0.79      0.80      0.76       300***

***Key Findings and Insights***
* Predictive Factors: Identification of significant predictors for fraud and claim amounts through correlation and cluster analysis.
* Model Performance: Discussion on the effectiveness of the regression and classification models, including the impact of SMOTE on classification accuracy.

# Conclusions
The notebook demonstrates a robust approach to understanding and predicting insurance fraud and claims using statistical analyses and machine learning. 
Recommendations for future work might include exploring more advanced machine learning algorithms or deeper feature engineering to improve model performance.
