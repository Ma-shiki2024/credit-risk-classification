# credit-risk-classification

In this Challenge , We used various techniques to train and evaluate a model based on loan risk . With the provided dataset , our goal was to build a model that can identify the creditworthiness of borrowers.

Credit-risk-classification and lending_data.csv are the two files that we used inside the credit risk folder .
The instructions for this challenge are divided into the following subsections :
Split the Data into training and training sets 
create a logistic Regression Model with the Orginal data 
Write a credit risk Analysis Report 


Stages of the machine learning process:
Data Split:

The dataset was split into training and testing sets to evaluate the model's performance.
The dataset was split into training and testing sets to evaluate the model's performance.

Model Training:

Initialize Logistic Regression Model. The first logistic regression model was constructed using the original dataset, which consisted of 75,036 data points classified as low risk and 2,500 data points classified as high risk. The objective of this model was to predict the classification (low risk or high risk) of loans given to borrowers in the testing set.
Used the training data to fit the model to the data.
During training, the algorithm adjusts the model's weights to minimize the logistic loss between the predicted probabilities and the actual binary labels.
Resampling with RandomOverSampler:

To tackle the issue of class imbalance, the training data underwent resampling using the RandomOverSampler technique. This approach ensured an equal representation of both low-risk and high-risk labels by increasing the number of high-risk data points. As a result, both classes consisted of 56,277 data points each after the resampling process.
Logistic Regression Model with Resampled Data:

A logistic regression model was constructed using the resampled data. The objective of this model was to predict loan risk based on the training data that underwent the resampling process.

Model Evaluation:

Used the validation set to evaluate the model's performance using appropriate metrics such as accuracy, precision, recall, and F1-score.
The objective of these steps was to evaluate and compare the performance of two logistic regression models. The first model was trained on the original data, while the second model was trained on the resampled data. By conducting this comparison, the effectiveness of resampling in addressing class imbalance and enhancing the model's predictive capabilities for loan risk classification could be assessed.

Results

Machine Learning Model 1:

For the Healthy Loans (0), the precision is 1.00, indicating that all the predictions for this label were correct. The recall is 1.00, meaning that all instances of this label were correctly identified.
The precision for High-Risk Loan (1) is 0.87, indicating that 87% of the predictions for this label were accurate. The recall is 0.89, indicating that 89% of the instances of this label were correctly identified.
The overall accuracy of the model is 0.99, indicating that it correctly predicted the loan risk for 99% of the instances.
Machine Learning Model 2:

The prescision is 87% and recall is at 89%, which indicates a high rate of correct identification of high-risk loans with a small number of false positives.
The overall accuracy of the model is 0.99, indicating that it correctly predicted the loan risk for 99% of the instances.
Summary
Upon analysis, it was observed that both models exhibited commendable accuracy, precision, and recall scores. However, the logistic regression model that utilized resampling showcased a slightly superior performance, achieving an accuracy score of 0.9945 compared to 0.9924 for the initial logistic regression model.

Considering the objective of accurately identifying both healthy loans and high-risk loans, the logistic regression model with resampling emerges as the optimal choice.