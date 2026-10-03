# Student Performance Prediction Using Logistic Regression

## Project Overview

This is a beginner machine learning project focused on predicting whether a student will **Pass or Fail** based on selected academic performance indicators.

This project is part of my learning journey in **Python, Data Analysis, and Machine Learning**.

## Project Objective

The goal of this project is to build a classification model that predicts a student's result using:

- Hours studied
- Attendance
- Assignment score

## Dataset

The dataset contains 19 student records with the following variables:

- **Student** — Student identifier
- **Hours_studied** — Number of hours studied
- **attendance** — Student attendance
- **assignment_Score** — Assignment score
- **result** — Pass or Fail

## Data Preparation

I inspected the dataset using Pandas and checked for missing values using `isnull().sum()`.

Missing numerical values were handled using `SimpleImputer` with the mean strategy.

## Features and Target

The following variables were used as features:

- Hours studied
- Attendance
- Assignment score

The target variable was:

- Result — Pass or Fail

The Student column was not used as a predictive feature because it is an identifier rather than a meaningful predictor.

## Machine Learning Model

Since the target variable contains two categories (Pass and Fail), this is a **classification problem**.

I used **Logistic Regression** as the machine learning algorithm.

The model was configured with:

```python
LogisticRegression(max_iter=1000)
```

The dataset was divided into training and testing sets using an 80/20 split.

## Model Evaluation

The model correctly predicted **3 out of 4** observations in the test set.

This resulted in an accuracy of:

**75%**

### Confusion Matrix

The confusion matrix was:

```text
[[2 1]
 [0 1]]
```

This shows that the model correctly classified 3 of the 4 test observations and incorrectly classified 1.

A classification report was also generated to examine:

- Precision
- Recall
- F1-score
- Support

Because the dataset contains only 19 observations and the test set contains only 4 observations, the 75% accuracy should be interpreted cautiously. A larger dataset would provide a more reliable evaluation.

## Key Learning Outcomes

Through this project, I practiced:

- Creating and exploring a dataset
- Using Pandas
- Detecting missing values
- Handling missing values with SimpleImputer
- Selecting features and target variables
- Splitting data into training and testing sets
- Building a Logistic Regression model
- Making predictions
- Evaluating a classification model
- Understanding accuracy
- Understanding confusion matrices
- Generating a classification report
- Documenting a machine learning project

## Future Improvements

I would like to improve this project by:

- Using a larger dataset
- Exploring additional classification models
- Comparing different machine learning models
- Adding data visualizations
- Exploring additional evaluation metrics
- Improving feature selection

## Tools Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook
- GitHub