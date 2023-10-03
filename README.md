# BIOS667
README: Lung Cancer Prediction
Overview
This analysis, carried out by Sakshi Garg, aims to predict lung cancer using both supervised and unsupervised machine learning techniques. The dataset used contains details related to demographic and clinical features of 1000 lung cancer patients.

Background

Lung cancer is the leading cause of cancer-related deaths worldwide. There are primarily two types: non-small cell lung cancer (NSCLC) and small cell lung cancer (SCLC). This analysis focuses on developing models to predict the likelihood and severity of lung cancer based on predictors such as age, sex, smoking status, and more.

Dataset Source

Data has been sourced from Kaggle: Lung Cancer and Air Pollution.

The dataset contains:

1000 rows with each row corresponding to a unique lung cancer patient.
Gender representation: 1 = male, 2 = female.
A column indicating the severity of the disease.

Analysis Steps

1. Data Cleaning:
Loaded necessary R libraries like caret and tidyverse.
Renamed columns to more meaningful names.
Converted character values to factors and summarized data.
Checked for correlations between variables.
2. Supervised Learning:
Split the dataset into a 70:30 train-test ratio.
Trained a multinomial classification model to predict the presence of lung cancer.
Used penalized logistic regression and random forest algorithms.
Evaluated models using confusion matrices.
3. Unsupervised Learning:
Performed Principal Component Analysis (PCA) for dimensionality reduction.
Conducted k-means clustering to identify potential patient subpopulations.
Visualized PCA and k-means results for insights.

Results

Logistic Regression: High accuracy with only one misclassification.
Random Forest: Achieved perfect accuracy on test data. Noted potential overfitting.
PCA: First two principal components explained approximately 50% of the variation.
K-means Clustering: Identified 7 patient clusters. Clusters 1, 2, 3, and 6 correctly predicted lung cancer levels.

Insights

Smoking, obesity, air pollution, coughing of blood, and being a passive smoker are strong predictors of lung cancer.
The attribute "balanced diet" emerged as an odd predictor of lung cancer, suggesting potential dataset discrepancies.
Random forest slightly outperformed penalized logistic regression.

Concluding Remarks

This analysis provides a foundational understanding of the variables contributing to lung cancer. While models achieved high accuracy, further investigation into the dataset, especially concerning the attribute "balanced diet", is recommended.

References

Anil Kumar, C. et al. (2022). Lung Cancer Prediction from Text Datasets Using Machine Learning.
Brocken P., et al. (2012). Timeliness of lung cancer diagnosis and treatment.
Dela Cruz, C. S., et al. (2011). Lung cancer: epidemiology, etiology, and prevention.
Hirakata Y, Kitamura S. (1995). Pulmonary hypertrophic osteoarthropathy and clubbing of fingers in patients with lung cancer.
