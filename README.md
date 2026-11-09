# Air Quality Prediction Using Machine Learning

## Project Overview

This project focuses on analysing air quality data and developing machine learning classification models to predict air quality categories based on various air pollutant measurements. The dataset contains air quality observations from different cities in India, including pollutant concentrations such as PM2.5, PM10, NO, NO2, CO, SO2, and O3.

The primary objective is to identify patterns in air pollution data and classify air quality into six categories: Good, Satisfactory, Moderate, Poor, Very Poor, and Severe.

## Project Objectives

- Analyse air quality data to understand pollution patterns and distributions.
- Perform data cleaning and preprocessing to handle missing values and categorical variables.
- Apply feature scaling using RobustScaler.
- Perform exploratory data analysis (EDA) using visualisations such as count plots and correlation heatmaps.
- Apply feature selection to identify relevant input variables.
- Build and compare multiple machine learning classification models.
- Perform hyperparameter tuning to improve model performance.
- Evaluate the models using appropriate classification metrics.

## Dataset

**Source:** [Air Quality Data in India – Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)

- Original dataset: 29,531 rows and 16 columns.
- Target variable: AQI_Bucket
- Problem type: Multiclass Classification.
- Target categories: Good, Satisfactory, Moderate, Poor, Very Poor, and Severe.

The AQ column was excluded from the input features to avoid target leakage, as the AQI category is derived from the AQI value.

## Technologies and Libraries

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. **Data Loading:** Import the dataset and understand its structure.
2. **Data Preprocessing:** Handle missing values and encode categorical variables.
3. **Exploratory Data Analysis:** Analyse feature distributions and correlations through visualisations.
4. **Feature Scaling:** Apply RobustScaler to numerical features.
5. **Feature Selection:** Use SelectKBest to identify important features.
6. **Model Building:** Implement multiple classification algorithms.
7. **Model Comparison:** Compare model performance using accuracy, precision, recall, and F1-score.
8. **Hyperparameter Tuning:** Use RandomizedSearchCV with cross-validation to identify suitable model parameters.
9. **Model Evaluation:** Evaluate the tuned models using test data and select the best-performing model.

## Machine Learning Algorithms

The following classification algorithms are considered:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- Weighted F1-score
- Macro F1-score

Macro F1-score is particularly useful for this project because the AQI categories are not equally represented in the dataset.

## Expected Outcome

The project aims to identify an effective classification model for predicting air quality categories based on pollutant measurements. By comparing multiple algorithms and optimising their hyperparameters, the project seeks to improve classification performance and provide insights into air pollution patterns across different cities in India.

## Conclusion

This project demonstrates the application of the end-to-end machine learning workflow, from data preprocessing and exploratory data analysis to model development, hyperparameter optimisation, and evaluation. It provides an opportunity to understand how machine learning techniques can be applied to environmental data to support air quality analysis and classification.
