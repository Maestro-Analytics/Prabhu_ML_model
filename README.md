# Prabhu_ML_model
Trained ML model for Prabhu bank
# KMeans Clustering Model
Problem Statement: Banks struggle to segment customers effectively, leading to generalized marketing and inefficiencies.

Solution: Using KMeans clustering to group customers based on financial behavior for personalized services and optimized resource allocation.

Input Features:

Numerical Columns:
annual_others_income, totalhouseholdincm, annual_salary_income, annual_total_income, dis_amt, kyc_flag.
Categorical Columns:
cust_age_index, category_occ_index, category_schm_index, employment_status_index, income_nature_index, riskrating_index, marital_status_index, kyc_flag.
Technical Details:

Python Version: > 3.10
Number of Clusters: 3
Purpose: Enables banks to enhance marketing strategies, optimize resources, and improve customer satisfaction through targeted segmentation.

Datasets:
'hdfs://localhost:9000/ingest/ml_dataset/gsa_lam_demo_int_table'

# Regression model
Problem Statement:struggle to predict disbursement amounts (dis_amt), leading to inefficiencies in financial planning and customer service.

Solution: A Linear Regression model predicts dis_amt based on customer financial and demographic features, enabling better resource allocation and service optimization.

Input Features:

Numerical:
annual_others_income, totalhouseholdincm, annual_salary_income, annual_total_income, kyc_flag
Categorical (Encoded):
cust_age_index, category_occ_index, category_schm_index, employment_status_index, income_nature_index, riskrating_index, marital_status_index, kyc_flag_index
Output Parameter:

dis_amt (predicted disbursement amount)
Technical Requirements:

Python Version: > 3.10
Libraries: pandas, numpy, scikit-learn

model=Linearregressor &randomforest regressor
dataset:
hdfs://localhost:9000/ingest/ml_dataset/gsa_lam_demo_int_table

# Risk analysis
Problem Statement: Banks face challenges in predicting risk ratings, which affects decision-making and resource allocation.

Solution: A Logistic Regression model predicts the label (risk rating) based on 12 months of financial data, enabling better risk assessment and resource optimization.

Input Features:

month_0, month_1, month_2, month_3, month_4, month_5, month_6, month_7, month_8, month_9, month_10, month_11, month_12
Output Column:

label (risk rating classification)
Technical Requirements:

Python Version: > 3.10
Libraries: pandas, numpy, scikit-learn

data:
hdfs://localhost:9000/machine_learning/trans_train_source/trans_hist_training

  
