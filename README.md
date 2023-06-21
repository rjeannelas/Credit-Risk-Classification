# Credit-Risk-Classification

### Split the Data into Training and Testing Sets
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
- Split the data into training and testing datasets by using train_test_split.

### Create a Logistic Regression Model with the Original Data
- Fit a logistic regression model by using the training data (X_train and y_train).
- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance by doing the following:
  - Generate a confusion matrix.
  - Print the classification report.
  - 
Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

### Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that was used. 
Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:

#### Overview


#### Results
<img width="281" alt="Original Data" src="https://github.com/rjeannelas/Credit-Risk-Classification/assets/119624099/e1dba558-cb49-4704-8725-4795a5d10a51">




#### Summary

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.
