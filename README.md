Heart-Disease-Prediction
The primary objective of this project was to build a predictive system that can accurately determine if a patient has heart disease

Objective: Build a system that can predict if a patient has heart disease. Explore the data, understand the features, and figure out an approach.

Dataset: This dataset contains data about patient vitals and heart disease(if any) of the same.

Methodology: The project was executed in three main phases: Phase 1: Exploratory Data Analysis (EDA) We first explored the data to uncover patterns. This involved: Checking the balance of the target variable to see if our dataset was skewed (it was fairly balanced). Visualizing the distributions of key features like age, cholesterol, and max heart rate for patients with and without heart disease. Plotting how categorical features like sex and chest pain type correlate with a heart disease diagnosis. Creating a correlation heatmap to understand how all numerical features relate to each other and to the target.

Phase 2: Data Preprocessing To prepare the data for machine learning, we: Converted Categorical Data: Used one-hot encoding (via pd.get_dummies) to convert categorical columns (like chest pain type) into a numerical format that models can understand. Split the Data: Divided the dataset into a training set (80%) to teach the models and a testing set (20%) to evaluate their performance. Feature Scaling: Applied StandardScaler to all numerical features. This normalizes the data, ensuring that features with larger ranges (like cholesterol) do not unfairly dominate features with smaller ranges (like oldpeak).

Phase 3: Model Building and Evaluation We trained and evaluated three different classification models to find the most effective "system" for prediction. Logistic Regression: A solid, reliable baseline model for binary classification. Random Forest Classifier: A powerful ensemble model that builds multiple decision trees and combines their votes. XGBoost Classifier: A highly advanced and often top-performing gradient-boosting model. Each model was trained on the X_train data and then tested on the unseen X_test data. We measured their performance using accuracy, precision, recall, and a confusion matrix.

Conclusion: The Random Forest model provided the highest accuracy at 94.12%, making it the most effective "system" for predicting heart disease from this dataset. A feature importance analysis from the Random Forest model also revealed that ST slope, chest pain type, max heart rate, and oldpeak were among the most influential factors in its predictions.
