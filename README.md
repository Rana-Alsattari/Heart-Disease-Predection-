# Heart Disease Predection 
# Heart Disease Prediction – Data Engineering and Machine Learning Pipeline

This repository contains a complete end-to-end pipeline for predicting heart disease using structured medical and lifestyle data. The project includes extraction, cleaning, feature engineering, integration, scaling, model training, evaluation, and final predictive visualizations. The full academic report documenting every phase is included in the repository.

---

## Repository Structure

```
DataProjectOutputs/
│
├── phase1_extraction_simple
├── phase2_before_cleaning
├── phase2_after_cleaning
├── phase3_feature_engineering
├── phase3_integration
├── phase3_scaling
├── phase3_visualizations
├── phase4_feature_selection_fixed
├── phase4_visualizations
├── phase5_chi_squared
├── phase6_model_comparison
└── phase7_visual_dashboard

DE_Final.ipynb
Heart Disease Prediction Report.pdf
Medicaldataset.csv
README.md
data_missing.csv
data_missing_medical.csv
heart_dataset_cleaned.csv
heart_dataset_invalid.csv
heart_disease_dataset.csv
medical_dataset_cleaned.csv
medical_dataset_invalid.csv
```

Each folder contains outputs, intermediate datasets, visualizations, or logs generated during each pipeline phase.

---

## 1. Introduction

This project applies a full data engineering and machine learning workflow to predict heart disease. The goal is to transform raw medical datasets into a clean, merged, and analysis-ready dataset and to train predictive models capable of identifying patterns associated with heart disease.

---

## 2. Project Description

The project uses two Kaggle datasets: a heart dataset and a clinical medical dataset. The workflow includes raw data extraction, profiling, cleaning, outlier handling, missing value imputation, encoding, feature engineering, dataset merging, scaling, model training, and visual dashboard creation. Two models were trained and compared: Random Forest and Logistic Regression.

---

## 3. Pipeline Overview

### Phase 1 – Extraction  
Folder: `phase1_extraction_simple`  
Initial dataset loading, basic metadata inspection, and raw profiling.

### Phase 2 – Cleaning  
Folders:  
- `phase2_before_cleaning`  
- `phase2_after_cleaning`  

Includes:  
- Injecting missing and invalid values  
- Duplicate detection  
- Missing value imputation  
- Outlier correction  
- Label encoding  
- Column normalization  

### Phase 3 – Feature Engineering, Integration, Scaling  
Folders:  
- `phase3_feature_engineering`  
- `phase3_integration`  
- `phase3_scaling`  
- `phase3_visualizations`  

Includes:  
- Creating lifestyle_score, risk_score, age_group  
- Merging datasets using age and gender  
- Scaling with StandardScaler and MinMaxScaler  
- Visual distribution and correlation plots  

### Phase 4 – Feature Selection  
Folders:  
- `phase4_feature_selection_fixed`  
- `phase4_visualizations`  

Includes:  
- Correlation filtering  
- Random Forest feature importance  
- Removal of redundant or low-importance features  

### Phase 5 – Statistical Tests  
Folder: `phase5_chi_squared`  
Categorical significance testing using chi-squared statistics.

### Phase 6 – Model Comparison  
Folder: `phase6_model_comparison`  

Models trained:  
- Random Forest  
- Logistic Regression  

Results include:  
- Confusion matrices  
- Feature importance comparison  
- Classification metrics  
- Accuracy comparison  

### Phase 7 – Visual Dashboard  
Folder: `phase7_visual_dashboard`  

Includes ROC curve, probability distribution, and final performance charts.

---

## 4. Datasets Included

The following datasets are provided for complete transparency and reproducibility:

- Medicaldataset.csv  
- heart_disease_dataset.csv  
- heart_dataset_cleaned.csv  
- heart_dataset_invalid.csv  
- medical_dataset_cleaned.csv  
- medical_dataset_invalid.csv  
- data_missing.csv  
- data_missing_medical.csv  

Each dataset corresponds to a different processing stage within the pipeline.

---

## 5. Notebook

`DE_Final.ipynb` contains the full step-by-step pipeline, including data loading, transformations, feature engineering, integration, model training, and visualizations.

---

## 6. Visualizations

All visual outputs generated throughout the pipeline are stored within the corresponding phase folders in `DataProjectOutputs`.  
After uploading images to GitHub, you may insert them using the following format:

```
![Title](DataProjectOutputs/phase3_visualizations/your_image_name.png)
```

---

## 7. How to Reproduce

1. Install the required Python libraries.
2. Open and run `DE_Final.ipynb` sequentially.
3. Review intermediate outputs inside `DataProjectOutputs`.
4. Compare model performance using the results in `phase6_model_comparison`.
5. View the final dashboard outputs in `phase7_visual_dashboard`.

---

## 8. Report

The full project documentation, including methodology, transformations, visualizations, and evaluation, is available in:

`Heart Disease Prediction Report.pdf`

---

## 9. Conclusion

The repository provides a complete data engineering pipeline for heart disease prediction, from raw data to final model performance dashboards. It demonstrates structured cleaning, transformation, merging, feature engineering, modeling, and visualization techniques, resulting in a reproducible and well-organized workflow.

