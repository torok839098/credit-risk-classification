# credit-risk-classification

Using various techniques to train and evaluate a model based on loan risk. Use the dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Before beginning the analysis (based on instructions):

-Clown new repository with name of Module

-Download the Module Files and create a folder titled "Credit_Risk."

-Inside the "Credit_Risk" folder, add the credit_risk_classification.ipynb and lending_data.csv files found in the "Starter_Code.zip" file.

-Push your changes to GitHub.


# Part One: Train and Evaluate The Model 

The purpose of this analysis is credi-risk classifiction by determining the loan status as 'high-risk'(1) and healthy loan (0). Several models will and reports will be made to determine such status.


## Split the Data into Training and Testing Sets:

Step 1: Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

Step 2: Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

Step 3: Check the balance of the labels variable (y) by using the value_counts function.

Step 4: Split the data into training and testing datasets by using train_test_split.

## Create a Logistic Regression Model with the Original Data

Step 1: Fit a logistic regression model by using the training data (X_train and y_train).

Step 2: Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model.

Step 3: Evaluate the model’s performance by doing the following:

  -Calculate the accuracy score of the model.

  -Generate a confusion matrix.

  -Print the classification report.

## Predict a Logistic Regression Model with Resampled Training Data

Step 1: Use the RandomOverSampler module from the imbalanced-learn library to resample the data. Be sure to confirm that the labels have an equal number of data points.

Step 2: Use the LogisticRegression classifier and the resampled data to fit the model and make predictions.

Step 3: Evaluate the model’s performance by doing the following:

-Calculate the accuracy score of the model.

-Generate a confusion matrix.

-Print the classification report.

# Part 2: Written Report
Things to consider when writting the report: 

Overview of analysis:
* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

For the Results section:

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:Logistic Regression Model with the Original Data
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
* Machine Learning Model 2:Logistic Regression Model with Resampled Training Data
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
For the Summary Section: 

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

## References

Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
For additional references, see the starter code. Instructions are based on report and module requirements. 
