# Recipe-Reviews-and-User-Feedback

Project Overview
This project focuses on analyzing recipe reviews and user feedback to predict user ratings using machine learning classification algorithms. The dataset contains information about recipes, user interactions, review comments, and ratings.
The main objective is to understand user feedback patterns and build classification models that predict recipe ratings based on review text and numerical features.

Dataset Description
Dataset Name: Recipe Reviews and User Feedback Dataset
Total Records: 18,182
Total Original Columns: 15
Target Variable: stars
Target Classes: 0, 1, 2, 3, 4, 5

Features Used
text – User review comments
user_reputation – User reputation score
reply_count – Number of replies
thumbs_up – Positive feedback count
thumbs_down – Negative feedback count

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook

Project Workflow

1. Data Loading and Exploration
Loaded the dataset using Pandas.
Examined dataset dimensions and column names.
Checked data types, missing values, and unique values.
Analyzed the distribution of user ratings.

2. Data Preprocessing
Removed unnecessary columns.
Converted numerical columns into appropriate data types.
Handled missing values.
Applied TF-IDF Vectorization to review text.
Used Simple Imputer and StandardScaler for numerical features.

3. Exploratory Data Analysis
Visualized the distribution of ratings.
Analyzed numerical feature distributions.
Examined relationships between user feedback and ratings.
Generated a correlation matrix to identify relationships among numerical variables.

4. Feature Selection
Applied SelectKBest with the ANOVA F-test (f_classif).
Selected the top 20 features.
Avoided data leakage by fitting preprocessing and feature selection only on the training data.

5. Model Building and Training
Implemented the following classification algorithms:
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Class balancing was applied to help address the imbalance in rating classes.

6. Model Evaluation
Evaluated the models using:
Accuracy
Precision
Recall
F1-Score
Weighted averaging was used for multiclass evaluation.

Correlation Analysis
The correlation matrix showed that thumbs_up and best_score had the strongest positive correlation (approximately 0.685) among the numerical features.

Project Objective
To develop and compare machine learning classification models that predict recipe ratings using review text and user feedback information.

Conclusion
This project demonstrates the application of data preprocessing, exploratory data analysis, feature extraction, feature selection, and machine learning classification techniques to a real-world user feedback dataset.
The performance of Logistic Regression, Decision Tree, and Random Forest models is compared to identify a suitable classification approach for predicting recipe ratings.

Author
Bhargavi D
B.Sc. Computer Science with Artificial Intelligence
M.O.P. Vaishnav College for Women
