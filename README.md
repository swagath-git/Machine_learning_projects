# 1. Fuel Economy Analysis
Overview This project focuses on analyzing fuel economy data using machine learning techniques. The dataset contains various features related to vehicle specifications, fuel types, and fuel costs.

# Dataset :-
The dataset (vehicles.csv) used in this project consists of numerical and categorical fuel economy variables.

# Data Preprocessing :-
Imputation: Missing values in numerical columns are filled using the median value of each respective column. Outlier Removal: Outliers are identified and removed from the dataset based on the interquartile range (IQR) method. Scaling: Numerical features are scaled using both StandardScaler and MinMaxScaler techniques.

# Model Training :-
Three regression models are trained on the preprocessed dataset: Linear Regression Decision Tree Regressor Random Forest Regressor

# Evaluation :-
The trained models are evaluated using the R-squared (R2) metric on both training and testing datasets to assess their performance. R2 score measures the proportion of the variance in the dependent variable that is predictable from the independent variables.

# Results :-
Linear Regression: Achieved a training score of [0.99] and a testing score of [0.99]. Decision Tree Regressor: Achieved a training score of [1.0] and a testing score of [1.0]. Random Forest Regressor: Achieved a training score of [0.99] and a testing score of [0.99].

# Conclusion :-
All Models Performed well outperformed the other models with the highest testing score.


---


# 2. Titanic Survival Prediction
# Overview :-
This project aims to predict the survival of passengers aboard the Titanic using machine learning techniques. The dataset contains various features such as age, gender, ticket class, and cabin, which are used to train the models.

# Dataset :-
The dataset used in this project is provided as a CSV file named "Titanic.csv". It includes information about passengers aboard the Titanic, including whether they survived or not. The dataset contains both numerical and categorical features.

# Preprocessing :-
Loading the Dataset: Read the dataset using pandas. Handling Missing Values: For numerical columns, fill missing values with the median. For categorical columns, fill missing values with the mode. Outlier Removal: Identify outliers in numerical features. Remove outliers using the interquartile range (IQR) method. Feature Scaling: Scale numerical features using StandardScaler and MinMaxScaler. Feature Encoding: Encode categorical features using LabelEncoder. Model Training: Splitting the Data: Split the preprocessed data into training and testing sets (e.g., 70% training, 30% testing).

# Model Selection :-
Train three different classification models: Logistic Regression Decision Tree Classifier Random Forest Classifier.

# Results :-
The trained models achieve certain accuracy scores on both training and testing datasets, indicating their predictive

---

# Gradient Boosting Classification

## Project Overview

This project uses the **Mushroom dataset** to build a classification model using the **Gradient Boosting Classifier**.

The project covers data preprocessing, model training, hyperparameter tuning, feature importance analysis, and model evaluation using Python and Scikit-learn.

## Objectives

* Preprocess categorical mushroom data using one-hot encoding
* Split the dataset into training and testing sets
* Build a Gradient Boosting classification model
* Evaluate model performance using accuracy and cross-validation
* Identify the best hyperparameters using GridSearchCV
* Analyze important features
* Rebuild the model using selected important features
* Evaluate the final model using a confusion matrix and classification report

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## 🔄 Project Workflow

### 1. Data Loading

The `mushrooms.csv` dataset is loaded using Pandas.

### 2. Data Preprocessing

The target variable `class` is separated from the input features.

Categorical features are converted into numerical features using:

```python
pd.get_dummies()
```

### 3. Train-Test Split

The dataset is divided into training and testing sets using an 80:20 split.

### 4. Gradient Boosting Model

A `GradientBoostingClassifier` is trained using the default parameters.

Model performance is evaluated using:

* Training Accuracy
* Testing Accuracy
* 5-Fold Cross-Validation

### 5. Hyperparameter Tuning

`GridSearchCV` is used to find better values for:

* `n_estimators`
* `learning_rate`

The parameter combinations are evaluated using 5-fold cross-validation.

### 6. Feature Importance

Feature importance scores are extracted from the tuned Gradient Boosting model.

Features with importance greater than `0.01` are selected for the final model.

### 7. Final Model

A new Gradient Boosting model is trained using the important features and the selected hyperparameters.

### 8. Model Evaluation

The final model is evaluated using:

* Training Accuracy
* Testing Accuracy
* Cross-Validation Score
* Confusion Matrix
* Classification Report

## 📊 Model

**Algorithm:** Gradient Boosting Classifier


## 📌 Key Learning Outcomes

Through this project, I practiced:

* Data preprocessing
* One-hot encoding
* Train-test splitting
* Gradient Boosting
* Cross-validation
* Hyperparameter tuning
* GridSearchCV
* Feature importance
* Confusion matrix
* Classification report
* Model evaluation



# Note :-
This projects was developed primarily to improve my practical experience and build strong hands-on expertise in Machine Learning tools and workflows.

