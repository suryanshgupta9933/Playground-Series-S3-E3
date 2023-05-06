# Playground-Series-S3-E3

This repository aims to predict employee attrition using XGBoost, CatBoost, and LightGBM algorithms using model ensembling. The data was obtained from a Kaggle competition. You can find the competition [here](https://www.kaggle.com/competitions/playground-series-s3e3).

## Table of Contents
- [Data Preprocessing.](#Data-Preprocessing)
- [Feature Extraction.](#Feature-Extraction)
- [Model Building.](#Model-Building)
    - [XGBoost.](#XGBoost)
    - [CatBoost.](#CatBoost)
    - [LightGBM.](#LightGBM)
- [Model Evaluation.](#Model-Evaluation)
6. Model Ensembling
7. Deployment

## Data Preprocessing
The data was already clean and ready to use. The only preprocessing step was to map the object features that had binary values to 0 and 1. The object features were encoded using the `LabelEncoder` from the `sklearn.preprocessing` module.

## Feature Extraction
The use of feature extraction techniques such as `PCA` and `LDA` were not necessary as the number of features was not large. However, feature engineering was done to create new features from the existing ones and features and target were separated.

## Model Building

### XGBoost Regression
The XGBoost model was built using the `XGBRegressor` from the `xgboost` module. The model was trained using the default parameters and the accuracy score was 0.766.

### CatBoost Regression
- The CatBoost model was built using the `CatBoostRegressor` from the `catboost` module. The model was trained using the default parameters for 200 iterations.
- Stratified K-Fold cross-validation was used with 10 folds to train the model. The accuracy score was 0.846.

### LightGBM Regression
- The LightGBM model was built using the `LGBMRegressor` from the `lightgbm` module. The model was trained using the default parameters for 200 iterations.
- Stratified K-Fold cross-validation was used with 10 folds to train the model. The accuracy score was 0.812.
