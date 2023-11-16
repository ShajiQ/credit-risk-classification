The purpose of this analysis was to develop a model to predict credit risk based on financial information. The goal was to gauge the credit security of loans by analyzing features and patterns that indicate the risk of default.
The dataset contained financial information of loan applications. The target variable, loan_status indicated whether a loan was healthy or had a high risk of default.

Variables to Predict:
loan_status (Target Variable): Binary variable indicating the health of the loan (0: Healthy, 1: High-risk).

Stages of the Machine Learning Process:
Data Loading and Exploration: Loaded the dataset, examined its structure, and split it into training and testing sets.
Logistic Regression Model: Developed a logistic regression model using the original data and evaluated its performance.
Resampling Techniques: Employed random oversampling to address class imbalance and trained a logistic regression model on the resampled data.
Model Evaluation: Assessed the performance of each model using metrics such as accuracy, precision, recall, and F1-score.

Methods Used:
Logistic Regression: Utilized logistic regression as the primary classification algorithm.
Random Oversampling: Applied random oversampling to address the imbalance in the target variable.

Results
Machine Learning Model 1: Logistic Regression (Original Data)
  -Balanced Accuracy Score: 0.95
  -Precision (Class 0): 1.00
  -Precision (Class 1): 0.86
  -Recall (Class 0): 1.00
  -Recall (Class 1): 0.91
Machine Learning Model 2: Logistic Regression (Resampled Data)
  -Balanced Accuracy Score: 0.99
  -Precision (Class 0): 1.00
  -Precision (Class 1): 0.85
  -Recall (Class 0): 0.99
  -Recall (Class 1): 0.99

The two models demonstrate high accuracy and precision, indicating their effectiveness in predicting credit risk.
Model 2, trained on oversampled data, shows improved recall for both classes, suggesting better identification of high-risk loans.

My recommendation would be Model 2, the logistic regression model trained on resampled data, is better for its improved recall without sacrificing overall performance.
However, the best model depends on the specific objectives and consequences of false positives and false negatives.
Further fine-tuning and validation may be necessary based on the business context and requirements.
