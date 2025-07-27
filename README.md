# MSCS_634_Project2

## Regression Modeling and Performance Evaluation
### Project Overview
This project applies data mining and machine learning techniques to the Pima Indian Diabetes Dataset to analyze patterns and predict the likelihood of diabetes based on medical attributes. The objective is to implement regression, classification, clustering, and association rule mining to uncover insights and build predictive models.

###  Dataset Summary
Source: UCI Machine Learning Repository

Records: 768 female patients of Pima Indian heritage

Features:

Pregnancies

Glucose

Blood Pressure

Skin Thickness

Insulin

BMI

Diabetes Pedigree Function

Age

Target Variable: Outcome (0 = No Diabetes, 1 = Diabetes)

This dataset was chosen due to its real-world applicability and structured nature, making it suitable for both supervised and unsupervised learning tasks.

###  Project Steps
1. Data Preprocessing
Replaced zeros with NaN in biologically invalid columns.

Imputed missing values using column means.

Standardized features using StandardScaler.

2. Exploratory Data Analysis (EDA)
Used boxplots, heatmaps, and correlation matrices.

Identified strong correlations with glucose, BMI, and age.

3. Regression Modeling
Applied Linear, Ridge, and Lasso Regression.

RMSE and R² used for performance comparison.

Lasso provided sparse models highlighting key features.

4. Classification
Models: Decision Tree, k-NN, Naïve Bayes

Evaluation: Accuracy, Confusion Matrix, F1 Score, ROC Curve

Best Performing Model: k-NN with tuned k = 7

5. Clustering
Used K-Means (k=2) to distinguish diabetic vs non-diabetic groups.

Visualized clusters using PCA.

6. Association Rule Mining
Applied Apriori Algorithm.

Discovered rules such as:

{Glucose=High, BMI=High} → {Diabetic}

###  Key Findings
Glucose and BMI are the most important predictors of diabetes.

k-NN outperformed other classifiers with ~78% accuracy.

Clustering revealed clear separation between diabetic and non-diabetic profiles.

Association rules uncovered clinically intuitive relationships in the data.

### Practical Recommendations
Use the k-NN classifier as a diagnostic aid in clinics.

Prioritize glucose and BMI monitoring in at-risk populations.

Consider deploying simple clustering tools for patient risk stratification.

###  Ethical Considerations
Dataset is anonymized; no personally identifiable data used.

Addressed potential bias by balancing the dataset and tuning models to prevent overfitting.

Used interpretable models for explainability in clinical settings.

### Conclusion
This end-to-end project demonstrates how machine learning and data mining techniques can derive actionable insights from healthcare datasets. With proper preprocessing and modeling, such tools can support real-world medical decision-making.

