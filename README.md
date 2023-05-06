# Playground-Series-S3-E3

This repository aims to predict employee attrition using XGBoost, CatBoost, and LightGBM algorithms using model ensembling. The data was obtained from a Kaggle competition. You can find the competition [here](https://www.kaggle.com/competitions/playground-series-s3e3).

## Table of Contents
- [Data Preprocessing.](#Data-Preprocessing)
- [Feature Extraction](#Feature-Extraction)
- Model Building
- Model Tuning
- Model Evaluation
- Model Ensembling
- Deployment

## Data Preprocessing
The data was already clean and ready to use. The only preprocessing step was to map object data types to integer data types. The following code was used to do so. Meaningless features were also dropped by checking their correlation with the one another.

## Feature Extraction
The use of feature extraction techniques such as PCA and LDA were not necessary as the number of features was not large. However, feature engineering was done to create new features from the existing ones and features and target were separated.