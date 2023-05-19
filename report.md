 # Module 12 Report Template

## Overview of the Analysis

* The two machine learning models used in this excercise are: A Logistic Regression with Original Data (using from sklearn.linear_model import LogisticRegression) and Logistic Regression Model with Resampled Training Data (using from imblearn.over_sampling import RandomOverSampler)

* The purpose of this analysis was for the bank to make a model to use two different models to predict the likehood a loan would be a good loan or a bad loan(high-risk loan). 


* The purpose of the analysis was to see which model was able to predict with greater accuracy the likelyhood that a loan would be good vs bad(high risk)

* The financial information the data was using was loan_size,interest_rate,borrower_income,debt_to_income,num_of_accounts,derogatory_marks,total_debt,loan_status and was used to predict Healthy Loans vs Non-Healthy Loans against their predicted counterparts.

* We were trying to predict Healthy Loans vs Non-Healthy loans in the most accurate way possible.

* Data was loaded in, seperated into the y (loan status) vs (X everything else), a Train Test Split was done, LogisticRegression and RandomOverSampler were used in the analysis, a Confusion Matrix was printed and a classification report was printed. All of these provided #s we can use to reach some conclusions about the models efficiency.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * A Logistic Regression with Original Data (using from sklearn.linear_model import LogisticRegression)
  * Scores -
   Balanced Accuracy Score: 0.9442676901753825
   Precision: 100% Healthy Loans / 87% Non Healthy Loans
   Recall: 100% / 89%

                      Predicted Healthy Loans	    Predicted Non-Healthy Loans
Health Loans	        18679	                      80
Non-Healthy Loans	    67	                        558


* Machine Learning Model 2:
  * Logistic Regression Model with Resampled Training Data (using from imblearn.over_sampling import RandomOverSampler)
  * Scores -
  Balanced Accuracy Score: 0.9959744975744975
  Precision: 100%  Healthy Loans / 0.87% Non Healthy Loans
  Recall: 100% / 100%

                      Predicted Healthy Loans	    Predicted Non-Healthy Loans
Health Loans	        18668	                      91
Non-Healthy Loans	    2	                          623

## Summary

* Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

The Second model preformed better as it was more accurate and eneded up predicting more correctly on the non preforming loans.

It is more important to predict the non-healthy loans as they are more likely to lose the institution money so the second model does better..

I would recomend using the second model as it seems to get better more accurate results than the first model on the bad performing loans. Which is super important when trying to prevent losing $.

Money matters to a bank/loan company so making sure to avoid bad debts would be one of the highest priorities for not losing money.

Getting the information wrong about the good clients by rejecting their loan application might be a risk to consider since their loan wasnt funded and interest income is not earned from them. But losing a total loan amount probably poses a greater risk than rejecting a few clients based on a better model. Further analysis would have to be completed.

The second model was 99.6% accurate vs the first model being 94.4% accurate. Those 5% matter when $ is at stake.
