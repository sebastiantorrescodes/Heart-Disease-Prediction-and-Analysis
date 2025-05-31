# Heart Disease Prediction and Analysis Using Machine Learning
# Overview  
This project applies a range of machine learning techniques to predict the presence of heart disease based on clinical and demographic data. The goal is to compare the effectiveness of different models and ensemble methods, and to provide a reproducible workflow for healthcare data analysis.  
# Dataset

The dataset used is heart.csv, which contains the following features for each patient:

* **Age:** Age of the patient:  
* **Sex:** Gender (M/F)
* **ChestPainType:** Type of chest pain (e.g., ATA, NAP, ASY, TA)
* **RestingBP:** Resting blood pressure (mm Hg)
* **Cholesterol:** Serum cholesterol (mg/dl)
* **FastingBS:** Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
* **RestingECG:** Resting electrocardiographic results (Normal, ST, LVH)
* **MaxHR:** Maximum heart rate achieved
* **ExerciseAngina:** Exercise-induced angina (Y/N)
* **Oldpeak:** ST depression induced by exercise relative to rest
* **ST_Slope:** Slope of the peak exercise ST segment (Up, Flat, Down)
* **HeartDisease:** Target variable (1 = presence; 0 = absence)
# Project Workflow
1. Data Loading and Exploration
    * Import the dataset and display sample records.
    * Check for missing values and data types.
2. Data Preprocessing
    * Encode categorical variables using one-hot encoding.
    * Split the data into training and testing sets (70/30 split).
3.Modeling and Evaluation
    * Decision Tree Classifier
      * Train and evaluate using both holdout and cross-validation methods.
    * Bagging Ensemble
      * Apply bagging with decision trees and evaluate with out-of-bag and test scores.
    * Random Forest Classifier
      * Perform 30-fold cross-validation to assess model robustness.
    * K-means Clustering
      * Explore unsupervised clustering for pattern discovery.
4. Performance Metrics
    * Accuracy scores for each model and method.
    * Cross-validation results for model comparison.
5. Visualization
    * Scatter plot matrix and other visualizations to understand feature relationships and model performance.
# Results
  * The notebook reports accuracy and cross-validation scores for each model.
  * Ensemble methods (Bagging, Random Forest) generally outperform single decision trees.
  * The workflow demonstrates the importance of preprocessing and model selection in healthcare analytics.
