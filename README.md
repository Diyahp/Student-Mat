
<h1>About Dataset</h1>
This dataset is downloaded from The UCI Machine Learning Repository is a collection of databases, domain theories, and data generators that are used by the machine learning community for the empirical analysis of machine learning algorithms.
This data approach student achievement in secondary education of two Portuguese schools. The data attributes include student grades, demographic, social and school related features) and it was collected by using school reports and questionnaires. Two datasets are provided regarding the performance in two distinct subjects: Mathematics (mat) and Portuguese language (por). In [Cortez and Silva, 2008], the two datasets were modeled under binary/five-level classification and regression tasks. Important note: the target attribute G3 has a strong correlation with attributes G2 and G1.
# Student Performance Prediction Project

## Project Overview

This project aims to analyze a student performance dataset to understand the factors influencing student academic outcomes, specifically the final grade (G3). We employ data cleaning, feature engineering, statistical analysis, and machine learning techniques to explore relationships and build a predictive model.

## Project Goals

* Load and explore the student performance dataset.
* Clean the data by handling outliers and inconsistencies.
* Analyze the relationships between different features and student performance (G1, G2, G3).
* Engineer new features to potentially improve model performance.
* Train and evaluate a linear regression model to predict the final grade (G3).
* Visualize key findings to gain insights into student performance.

## Methodology

This project follows a comprehensive data science pipeline:

1.  **Data Loading:**
    * Loading the student performance dataset into a pandas DataFrame.
    * Displaying the first few rows and DataFrame information for initial exploration.

2.  **Data Cleaning:**
    * Handling outliers in numerical features using box plots and the IQR method.
    * Standardizing categorical features to address inconsistencies.
    * Validating the cleaned data for accuracy.

3.  **Data Analysis:**
    * Calculating correlation between numerical features and G3.
    * Visualizing the correlation matrix using a heatmap.
    * Exploring relationships between categorical features and G3 using box plots.
    * Performing ANOVA tests for categorical features showing potential differences in G3.
    * Performing T-tests to compare male and female student grade differences.

4.  **Data Visualization:**
    * Creating correlation heatmaps, box plots, and scatter plots to visualize key findings.

5.  **Feature Engineering:**
    * Engineering new features, including study time ratio, combined grade score, and binary categorical features.
    * Exploring potential interactions between features, specifically weekly study time and extra educational support.

6.  **Data Splitting:**
    * Splitting the dataset into training and testing sets.

7.  **Model Training:**
    * Training a linear regression model to predict G3 based on engineered features.

8.  **Model Evaluation:**
    * Evaluating model performance using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R-squared (R2) score.

## Key Findings

* **Strong Correlation between G2 and G3:** G2 is a significant predictor of G3.
* **Negative Impact of Failures:** Failures negatively correlate with G3.
* **Statistically Significant Differences:**
    * ANOVA tests revealed significant differences in G3 based on 'address', 'Mother_job', 'internet_access', and 'romantic_relationship'.
    * A t-test showed significant differences in G3 between male and female students.
* **Model Performance:**
    * The linear regression model achieved an R2 score of 0.76, MSE of 4.84, RMSE of 2.20, and MAE of 1.49.
* **Feature Importance:**
    * G2 and G1 are strong predictors; failures and romantic relationships negatively impact G3.

## Questions Answered

* What is the relationship between different features and student performance (G1, G2, G3)?
* What is the performance of the trained linear regression model?
* Which features are most important for predicting the final grade (G3)?

## Tools Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib
* Scikit-learn (sklearn)
* SciPy
