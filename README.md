# Applied Machine Learning Projects

This repository contains practical machine learning projects that explore predictive modeling, computer vision, and statistical analysis. Each project folder maintains its datasets alongside the documented notebook workflows.

## 1. Cervical Cancer Risk Prediction
**Folder:** `cervical_cancer_risk_analysis/`  
**Task:** Imbalanced Binary Classification  

This project tackles a highly imbalanced medical classification task forecasting cervical cancer biopsy outcomes based on patient risk factors and demographics.

**Methodology Highlights:**
* **Leakage-Free Validation Pipeline:** Ensures scaling and imputation (median) are fit explicitly on training bounds.
* **Class Imbalance Mitigation:** Leverages **SMOTE** exclusively on training subgroups to anchor minority detection properly.
* **Algorithms Examined:** Random Forest, SVM (RBF), Decision Trees, Logistic Regression (L1 & L2 penalties).
* **Operating Threshold Tuning:** Uses independent validation distributions to identify probabilistic thresholds maximizing **Recall (Sensitivity)** without sacrificing algorithmic stability (measured via F1-Score cutoffs).
* **Comprehensive Metrics:** Includes dynamic PR-AUC curves and standardized confusion matrices evaluating diagnostic capabilities objectively.

## 2. MNIST Digit Classification
**Folder:** `classification/`  
**Task:** Multi-Class Image Classification  

A specialized computer vision pipeline focused on reading, authenticating, and classifying handwritten digits (0-9) originating from the classic MNIST dataset. Explores structured pixel processing, array reshaping, and foundational image recognition techniques scaled to multiclass categorical environments. 

## 3. Applied Linear Regression
**Folder:** `linear regression/`  
**Task:** Continuous Variable Prediction (Univariate Regression)

This module investigates linear relationships defining primary continuous variables. The tasks include assessing statistical dependency, implementing base regressions, and mapping best-fit lines. 
* **Study Hours vs Grades:** Projects final academic performance markers mapped dynamically against invested studying durations.
* **Years of Experience vs Salary:** Analyzes financial compensation curves systematically modeled upon career tenure metrics.

## How to Execute

1. Clone the repository locally.
2. Launch the respective `.ipynb` notebook files using your preferred environment (Jupyter Lab, VS Code, or Google Colab).
3. Datasets are directly bundled within their corresponding directory dependencies. No external downloads are required. Run all cells sequentially.

