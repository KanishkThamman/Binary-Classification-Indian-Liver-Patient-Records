# README: Financial and Health Data Analysis

## Table of Contents

1. [Overview](#overview)
2. [Model Descriptions](#model-descriptions)
3. [Dataset Overviews](#dataset-overviews)
    - [Indian Liver Patient Records](#indian-liver-patient-records)
    - [Synthetic Financial Data for Fraud Detection](#synthetic-financial-data-for-fraud-detection)
4. [Analysis Processes](#analysis-processes)
    - [Liver Patient Records Analysis](#liver-patient-records-analysis)
    - [Fraud Detection Analysis](#fraud-detection-analysis)
5. [Model Performance and Problems](#model-performance-and-problems)
6. [Conclusion and Recommendations](#conclusion-and-recommendations)
7. [Graphs and Visualizations](#graphs-and-visualizations)

## Overview

This repository contains two distinct data analysis projects:
1. **Indian Liver Patient Records Analysis**: Aimed at predicting liver disease based on patient records.
2. **Synthetic Financial Data for Fraud Detection Analysis**: Focused on detecting fraudulent financial transactions using machine learning models.

Each project involves different datasets, methodologies, and challenges. This README provides a detailed description of both analyses, their datasets, methodologies, performance evaluations, and findings.

## Model Descriptions

### Indian Liver Patient Records Analysis
- **Goal**: Predict liver disease in patients based on medical records.
- **Techniques Used**: Decision Tree, Random Forest, Logistic Regression, XGBoost.

### Synthetic Financial Data for Fraud Detection
- **Goal**: Identify fraudulent transactions in financial data.
- **Techniques Used**: Various machine learning models with emphasis on handling imbalanced and biased datasets.

## Dataset Overviews

### Indian Liver Patient Records
The dataset consists of liver patient records from India, including features such as age, gender, bilirubin levels, enzyme levels, and protein levels. The goal is to predict the presence of liver disease.

### Synthetic Financial Data for Fraud Detection
The dataset includes synthetic financial transactions simulating real-world scenarios with a mix of legitimate and fraudulent activities. The primary challenge is the imbalance between the number of legitimate and fraudulent transactions.

## Analysis Processes

### Liver Patient Records Analysis

1. **Data Preprocessing**: Cleaning, handling missing values, normalizing data, and encoding categorical variables.
2. **Feature Selection**: Identifying important features using correlation and statistical tests.
3. **Model Training**: Training Decision Tree, Random Forest, Logistic Regression, and XGBoost models.
4. **Model Evaluation**: Using ROC curve and AUC score for evaluation.

### Fraud Detection Analysis

1. **Data Preprocessing**: Similar to the liver patient records, with additional focus on addressing imbalance and bias.
2. **Model Training**: Developing various machine learning models.
3. **Model Evaluation**: Focus on metrics like precision, recall, and F1 score, in addition to ROC and AUC.

## Model Performance and Problems

### Liver Patient Records

- **Imbalance**: The dataset had an imbalance between liver disease and non-liver disease cases.
- **Feature Noise and Redundancy**: Some features added noise and redundancy, affecting model performance.

### Fraud Detection

- **Imbalance**: Extreme imbalance between legitimate and fraudulent transactions.
- **Bias**: Inherent biases in the data generation process.
- **Model Performance**: High accuracy but misleading due to imbalance, emphasizing the need for metrics like precision, recall, and F1 score.

**Note**: Although the model for the biased data is very accurate, it is very biased and would not perform well in a real-world scenario.

## Conclusion and Recommendations

### Liver Patient Records Analysis

- **Data Balancing**: Apply techniques like oversampling/undersampling.
- **Bias Mitigation**: Address biases in data collection and processing.
- **Evaluation with Different Metrics**: Use precision, recall, and F1 score.
- **Continuous Monitoring**: Regularly update and retrain models with balanced data.

### Fraud Detection Analysis

- **Data Balancing**: Use techniques like SMOTE.
- **Bias Mitigation**: Address biases from data generation.
- **Advanced Feature Selection**: Use methods like RFE and feature importance ranking.
- **Regularization Techniques**: Apply L1 and L2 regularization.

## Graphs and Visualizations

### ROC Curve - Cumulative Performance for Liver Patient Records

![ROC Curve](/Indian%20Liver%20Patient%20Records/images/output.png)

### Accuracy Score Comparison for Liver Patient Records

![Accuracy Score Comparison](/Indian%20Liver%20Patient%20Records/images/accuracy.png)

### F1 Score Comparison for Liver Patient Records

![F1 Score Comparison](/Indian%20Liver%20Patient%20Records/images/F1%20score.png)

### Performance Metrics for Fraud Detection Models

### ROC Curve
![ROC Curve Image](/Synthetic%20Financial%20Data%20for%20Fraud%20Detection/images/ROC.png)

### Precision-Recall Curve
![Precision-Recall Curve Image](/Synthetic%20Financial%20Data%20for%20Fraud%20Detection/images/PRC.png)

These visualizations provide a comprehensive view of model performance, highlighting areas for improvement and guiding future work in developing robust predictive models.
