# Credit Risk Classification
  ## Overview of the Analysis
The purpose of this analysis is to investigate the effectiveness of 2 models trained to predict the creditworthiness for borrowers. The dataset used to train and test the models is taken from a peer-to-peer lending company and includes the size of the loan, the interest rate, the borrower's income, the debt-to-income ratio, number of accounts held by the borrower, derogatory marks of the borrower, total debt of the borrower, and the loan status.

The loan status data was extracted from the original dataset, and training and testing datasets were created to train and test the models. The first model maintained the unbalanced ratio of healthy and high-risk loans from the original dataset for training. The second model was trained on data prepared using the RandomOverSample module to ensure that the labels (healthy(0)/high-risk(1)) have an equal number of data points. After the the data was prepared, logistic regression models were created and trained to make predictions.

  ## Results
Machine Learning Model 1 (original):

Accuracy: 95%
Precision: healthy - 100% ; high-risk - 85%
Recall: healthy - 99% ; high-risk - 91%
Machine Learning Model 2 (resampled):

Accuracy: 99%
Precision: healthy - 100% ; high-risk - 84%
Recall: healthy - 99% ; high-risk - 99%

  ## Summary
Machine Learning Model 2 is recommended for its overall higher accuracy, and specficially its ability to correctly identify high risk loans 99% of the time, compared with 91% from Model 1.

See credit_risk_classification document for full analysis 


See link to learn more about RandomOverSampler: https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.RandomOverSampler.html
