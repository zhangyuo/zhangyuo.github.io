---
title: Luyipai Real Estate Valuation System
date: 2018-07-30
links:
  - type: site
    url: https://github.com/yourrepo/luyipai-estimation
tags:
  - Real Estate
  - Decision Tree
  - Stacking
  - Predictive Analytics
---

**Project Background:**
* Automated property valuation for assets on Luyipai platform.
* Addressed inefficiencies and low accuracy in manual property appraisals.

**Data Collection & Processing:**
* Data sources: Transaction data, listing data, neighborhood prices.
* Data cleaning: Outlier removal (3-sigma rule), missing value imputation, log transformation for normality.
* Feature engineering: Area segmentation, building age, decoration, floor, etc.

**Modeling & Optimization:**
* Regression algorithms: Linear Regression, Random Forest, GBDT, XGBoost, LightGBM.
* Hyperparameter tuning: Grid search + cross-validation for tree depth, number of trees, learning rate, min samples per leaf.
* Ensemble: Stacking of GBDT/XGBoost/LightGBM with linear regression.
* Addressed imbalance with resampling and probability smoothing.

**Workflow:**
1. Process raw data and feature engineering.
2. Train multiple regression models with optimized hyperparameters.
3. Fuse results from listing and transaction data.
4. Detect and correct valuation anomalies.

**Project Outcome:**
* Decision tree regression MAPE: 92%; stacking improved by 3%.
* Increased efficiency and reliability of property valuation, aiding auction asset assessment.

<!--more-->
