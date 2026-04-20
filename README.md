
# EV Battery State of Charge and State of Health Prediction

A data-driven machine learning framework developed to predict 
the State of Charge (SOC) and State of Health (SOH) of 
lithium-ion batteries. As electric vehicles become increasingly 
prevalent, accurate battery state estimation is essential for 
improving safety, extending battery lifespan, and ensuring 
reliable range prediction.

---

## Problem Statement
Traditional methods for estimating SOC and SOH such as Coulomb 
counting and equivalent circuit models struggle under real-world 
conditions including temperature variations, noise, and battery 
ageing. This project explores machine learning as a more 
accurate and adaptable alternative.

---

## Dataset
- Source: Kaggle (publicly available EV battery dataset)
- 1,900 samples with 22 features
- Key features: terminal voltage, battery current, temperature,
  internal resistance, state of charge, state of health, 
  cycle degradation, charging efficiency

---

## Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook
- Machine Learning: Supervised Learning, Regression Modelling,
  Feature Engineering

---

## Project Workflow
1. **Data Cleaning & Preprocessing**
   - Verified data integrity across 1,900 rows and 22 columns
   - Standardised column formats and checked for missing values

2. **Exploratory Data Analysis (EDA)**
   - Analysed distributions of SOC and SOH
   - Studied relationships between voltage, current, 
     temperature, and battery state
   - Generated correlation heatmaps for SOC and SOH features

3. **Feature Engineering**
   - Engineered cycle-level aggregated features to capture 
     long-term degradation patterns
   - Key features: mean temperature, voltage range, internal 
     resistance trends, thermal stress index, charging efficiency

4. **Model Development**
   - Built supervised machine learning regression models 
     for both SOC and SOH prediction
   - Compared two ensemble models to identify best performance
   - Applied MinMax scaling and 80/20 train-test split

5. **Model Evaluation**
   - Evaluated using MAE, RMSE and R² metrics
   - Both SOC and SOH models achieved strong predictive accuracy
   - Random Forest outperformed benchmark model for both tasks

---

## Key Findings
- Voltage is the strongest predictor of SOC
- Internal resistance and thermal stress are key indicators 
  of long-term battery health (SOH)
- Cycle-level feature engineering significantly improved 
  SOH prediction accuracy
- Machine learning proved more reliable than traditional 
  estimation methods for this dataset

---


## Author
Jayashree Rajagopal
