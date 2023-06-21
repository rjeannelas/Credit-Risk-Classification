# Credit-Risk-Classification

#### Split the Data into Training and Testing Sets
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
- Split the data into training and testing datasets by using train_test_split.

#### Create a Logistic Regression Model with the Original Data
- Fit a logistic regression model by using the training data (X_train and y_train).
- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance by doing the following:
  - Generate a confusion matrix.
  - Print the classification report.
    
Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

### Credit Risk Analysis Report
#### Overview
- The purpose of this analysis is to evaluate a model based on loan, by use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
- By implementing the Logistic Regression machine learning model to predict the probabilty of a good investment, financial information from the dataset such as loan size, interest rate, debt-to-income ratio, number of accounts, derogatory marks, and total debt are all necessary to make predictions. 
- The variables that was used to provide basic information, we targeted a column labeled loan_status that was used to predict with a 0 being a "healthy loan" or a 1 being a "high-risk loan" on a separate portion
- Following the instructions described above, the stages of the machine learning process used throughout the analysis would include more information while measuring from SKLearn:
 - balanced_accuracy_score, confusion_matrix, classification_report will be used to compare the two instances of the logisitic regression model.
 - train_test_split will be used to split training and testing data points.
 - cross_val_score will be used to test and pick the optimal solver for the model. from imblearn.over_sampling:
 - RandomOverSampler will be used to oversample the training dataset for the oversampled instance of the model.easuring from SKLearn
   
#### Results
* Machine Learning Model 1:
  * Based from the original dataset provided
  * The logistic regression model predicted 0 (healthy loan) with a score of 0.99 and 1 (high-risk loan) with a score of 0.85 are strong precisions

<img width="281" alt="Original Data" src="https://github.com/rjeannelas/Credit-Risk-Classification/assets/119624099/e1dba558-cb49-4704-8725-4795a5d10a51">

* Machine Learning Model 2:
  * Based from the resampled dataset of the original dataset
  * The logistic regression model used to predict both `0` (healthy loan) and `1` (high-risk loan) labels, has shown that there are false positive and false negative rates
  
<img width="269" alt="Resampled Data" src="https://github.com/rjeannelas/Credit-Risk-Classification/assets/119624099/e3dafbb4-d494-48e8-87b6-3fc0fd1243b7">

#### Summary
* From the predictions of the logistic regression model used on the resampled training data performed better in predicting instances of '1' (high-risk loans). It can also be shown that both models performed similar when predicting '0' (healthy loans). The initial model did not get enough training to both accurately and precisely predict high-risk loans.
* The goal is for the model to produce false negatives as little as possible. The chances of a risky loan being approved and the lender would be at higher risk for their consideration to be defaulted on. So in this case, would be important that the performance would depend on prediction of false negatives.
* Based from this sample dataset, using the Logistic Regression Model as a tool for predicting probabilty, it would be perfect to be used for credit or loan lending platforms. Potential customers would be able to check the probability of their loan or credit application being approved. Creating increase speeds of processing with applications, only if the model would produce as little false positives as possible.
