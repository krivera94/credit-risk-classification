# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

- Explain the purpose of the analysis.
- Explain what financial information the data was on, and what you needed to predict.
- Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
- Describe the stages of the machine learning process you went through as part of this analysis.
- Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis was to develop a machine learning model capable of predicting credit risk. Specifically, the model aimed to classify loans into two categories: healthy loans (0) and high-risk loans (1). The dataset used contained financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. Key variables to predict were the loan statuses, indicated as '0' for healthy loans and '1' for high-risk loans. A preliminary analysis of these variables included examining their value_counts to understand the distribution of healthy and high-risk loans in the dataset.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

- Machine Learning Model 1:
  - Description of Model 1 Accuracy, Precision, and Recall scores.
    Accuracy: Model showed an overall accuracy of 99%, indicating a high level of correctness in its predictions.

Precision: For healthy loans (0), the precision was almost 1.00, suggesting that the model was almost always correct when it predicted a loan as healthy. For high-risk loans (1), the precision was 0.85, indicating that 85% of loans predicted as high-risk were actually high-risk.

Recall: The model had a recall of 0.99 for healthy loans and 0.91 for high-risk loans, meaning it correctly identified 99% of healthy loans and 91% of high-risk loans.

F1-Score: The F1-scores were 1.00 for healthy loans and 0.88 for high-risk loans, showing a strong balance between precision and recall for both classes.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

- Which one seems to perform best? How do you know it performs best?
- Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The logistic regression model proved to be highly effective in predicting both healthy and high-risk loans. Its high accuracy, precision, and recall make it a valuable tool for credit risk assessment. Something to point out is its ability to identify high-risk loans, an important aspect in financial decision-making.

Given the model's accurate performance, it is recommended for use in practical applications where predicting loan risk is essential. The model's strength lies in its balanced performance across both loan categories, making it a reliable choice for credit risk classification.

While the model is already performing at a high level, further tuning and exploration of other models, such as Random Forest or Gradient Boosting, could be conducted for comparison and potential improvement.
