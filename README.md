# Predicting Loan Defaults with Machine Learning

## Table of Contents
- [Overview](#overview)
- [Data Source](#data-source)
- [Challenges](#challenges)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Feature Engineering](#feature-engineering)
- [Model Development](#model-development)
- [Results & Performance](#results--performance)
- [Future Enhancements](#future-enhancements)
- [Contributors](#contributors)
- [Contact](#contact)

## Overview
This project focuses on predicting **loan defaults** to optimize **loan approval processes** and **protect financial margins**. By using **cost-sensitive machine learning models**, the project minimizes the misclassification of high-risk loans and maximizes profitability.

## Data Source
- **SBA Loan Data**: Small Business Administration (SBA) loan dataset from **1987-2014**.
- **Third-Party Data**:
  - 3-Digit Zip Code Details
  - ZIP Code Location Data

## Challenges
- **Risk Uncertainty**: SBA guarantees loans, but banks still face default risks.
- **Regulatory Compliance**: Basel III mandates accurate **Probability of Default (PD)** estimation.
- **Data Limitations**: The dataset covers 1987-2014, making some insights outdated.

## Data Cleaning & Preparation
- **Dropped records with null values** in key variables like **MIS_Status**.
- **Corrected inconsistent data** in fields like **RevLineCr, City, and Zip Code**.
- **Updated state information** using ZIP code references.
- **Filled missing values** using appropriate business rules.

## Feature Engineering
- Created new variables such as:
  - **Industry Flag**: Categorized industries into major groups.
  - **Recession Flag**: Loans active during the 2007-2009 recession.
  - **SBA Portion**: Percentage of loan backed by SBA.
  - **Company Size**: Categorized based on employee count.
  - **Default Rate Bucket**: Classified states by default percentage.

## Model Development
- **Stratified Sampling**: Addressed class imbalance (**85% Paid in Full, 15% Charged-Off**).
- **Feature Transformations**:
  - **Log Transformation**: For loan amounts and terms.
  - **Label Encoding & One-Hot Encoding**: For categorical variables.
- **Machine Learning Models Tested**:
  - **Logistic Regression** (with Class Weights & Elastic Net)
  - **Random Forest**
  - **XGBoost**
  - **CatBoost**
  - **Bagging Classifier**
  - **Neural Networks**
  - **LDA & QDA**

## Results & Performance
- **Best Model: CatBoost** with an **ROC-AUC of 0.97**.
- **Optimal cutoff probability: 0.4056**, maximizing cumulative profit.
- **Achieved a maximum profit of $2.03 Billion** in validation testing.
- **High recall** ensures most high-risk loans are correctly classified.

![image](https://github.com/user-attachments/assets/ed19d04e-63ee-40e8-85a0-3c6c6c6691d3)

## Future Enhancements
- **Implement deep learning models** for enhanced accuracy.

## Contributors
- **Vinmathi Iyappan**
- **Dinesh Saraswat**
- **Garima Vijay**

## Contact
📧 **Email:** [vinmathi.iyappan@gmail.com](mailto:vinmathi.iyappan@gmail.com)  
🔗 **LinkedIn:** [Vinmathi-iyappan](https://linkedin.com/in//vinmathi-iyappan/)  
🖥 **GitHub:** [Vinmathiiyappan](https://github.com/Vinmathiiyappan)

