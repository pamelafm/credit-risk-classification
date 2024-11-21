# credit-risk-classification

# Overview of the Analysis

The purpose of this analysis is to evaluate the performance of two logistic regression machine learning models in predicting the credit risk associated with loans. The analysis was conducted on financial data, specifically focusing on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The objective was to predict the loan status, either as a healthy loan (0) or high-risk loan (1).

# The stages of the machine learning process in this analysis included:

- Splitting the data into training and testing datasets
- Creating and fitting a logistic regression model with the original data
- Evaluating the model's performance using accuracy, precision, and recall scores
- Resampling the data using RandomOverSampler to address class imbalance
- Creating and fitting another logistic regression model with the resampled data
- Evaluating the performance of the resampled model using the same metrics
- Methods used in this analysis include LogisticRegression and RandomOverSampler for resampling.

# Results
- Machine Learning Model 1: Logistic Regression with Original Data
-Description of Model 1 Accuracy, Precision, and Recall scores.
Accuracy: The overall accuracy of the model is 0.99, indicating that it correctly classifies 99% of the instances. Precision:

- Healthy loans (0): The model has a precision of 1.00, which means it's excellent at identifying true positives with very few false positives.
- High-risk loans (1): The model has a precision of 0.84, indicating its moderate effectiveness in identifying high-risk loans with some false positives. Recall:
- Healthy loans (0): The model has a recall of 1.00, which means it's correctly identifying nearly all instances of healthy loans with very few false negatives.
- High-risk loans (1): The model has a recall of 0.94, indicating its effectiveness in identifying high-risk loans with some false negatives.

Based on the analysis provided, I would recommend this machine learning model, particularly the logistic regression model using the original data, for several reasons:

1. High Accuracy: The model achieved an overall accuracy of 0.99, indicating that it correctly classifies 99% of instances. This level of accuracy suggests that the model is highly reliable in its predictions.

2. Excellent Precision for Healthy Loans: The precision for healthy loans (0) is 1.00, which means the model is exceptional at identifying true positives with virtually no false positives. This is crucial in financial contexts, where falsely classifying a healthy loan as high-risk could lead to unnecessary denial of credit.

3. Moderate Precision for High-Risk Loans: While the precision for high-risk loans (1) is 0.84, indicating some false positives, it still reflects a reasonable ability to identify high-risk loans. In financial applications, it's often more acceptable to have some false positives than to miss high-risk loans, which could lead to significant losses.

4. Strong Recall for Healthy Loans: The recall for healthy loans is also 1.00, meaning the model correctly identifies nearly all healthy loans. This ensures that the majority of good borrowers are recognized, minimizing the risk of rejecting credit-worthy applicants.

5. Good Recall for High-Risk Loans: The recall for high-risk loans is 0.94, showing that the model effectively identifies a large portion of high-risk loans. This is important for managing credit risk and preventing potential defaults.

6. Data Resampling: The analysis also demonstrates an understanding of class imbalance by using RandomOverSampler, which can improve model performance in scenarios where one class is underrepresented. This technique can enhance the model's ability to generalize and make accurate predictions across both classes.

# CONCLUSION

Overall, the model demonstrates strong performance metrics, particularly in accurately classifying healthy loans and effectively identifying high-risk loans. Given these strengths, it would be appropriate to recommend this logistic regression model for predicting credit risk associated with loans. However, continuous monitoring and validation with new data would be essential to ensure its ongoing effectiveness and adaptability to changing patterns in loan data.
