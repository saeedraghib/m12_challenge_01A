# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.<br>
<b>Answer</b>: The purpose of this analysis is to determine whether oversampling of minority class makes any difference or not.
* Explain what financial information the data was on, and what you needed to predict.<br>
<b>Answer</b>: The data was on the loans being either 'high risk' or 'low risk'. The aim of this project was to predict 'recognition of high risk' loans.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).<br>
<b>Answer</b>: <br>
<i><u>value_counts</u></i>: gives the total count of the two classes.<br>
<i><u>X_train</u></i>: part of the original 'feature' data that will be used to train the model.<br>
<i><u>y_train</u></i>: part of the original 'target' data that will be used to train the model.<br>
<i><u>X_test</u></i>: part of the original 'feature' data that will be used to predict the model.<br>
<i><u>y_test</u></i>: part of the original 'target' data that will be used to test the model.<br>
<i><u>training_matrix</u></i>: creates a 'confusion matrix' and shows the number of 'True Posotives', 'False Negatives', 'False Positives' and 'True Negatives for the training data'.<br>
<i><u>test_matrix</u></i>: creates a 'confusion matrix' and shows the number of 'True Posotives', 'False Negatives', 'False Positives' and 'True Negatives for the test data'.<br>
<i><u>training_report</u></i>: shows the classification report for training data.<br>
<i><u>testing_report</u></i>: shows the classification report for testing data.<br>
<i><u>X_resampled</u></i>: holds the data for oversampling for features.<br>
<i><u>y_resampled</u></i>: holds the data for oversampling for target.<br>
<i><u>bas_rs</u></i>: holds the accuracy value for resampled data<br>
* Describe the stages of the machine learning process you went through as part of this analysis.<br>
<b>Answer</b>: The stages in this entire process were:<br>
<ul>
    <li>Split data into 'train' and 'test' data.</li>
    <li>Use 'model', 'fit' and 'predict' pattern to train data.</li>
    <li>Evaluate and analyze to see if the model improved or not.</li>
    <li>Write, this report.</li>
</ul>    
<br>
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
<b>Answer</b>: The methods that were used are:<br>
<ul>
    <li>read_csv().</li>
    <li>head() and tail().</li>
    <li>drop().</li>
    <li>value_counts()</li>
    <li>train_test_split()</li>
    <li>LogisticRegression()</li>
    <li>fit()</li>
    <li>predict()</li>
    <li>accuracy_score()</li>
    <li>confusion_matrix()</li>
    <li>classification_report()</li>
    <li>RandomOverSampler()</li>
    <li>fit_resample()</li>
    <li>balanced_accuracy_report()</li>
</ul>    
<br>

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
<ul>
    <li>Accuracy: ... shows the 'True Positives' and 'True Negatives'.</li>
    <li>Precission: ... shows the ability of detecting 'high risk' loans.</li>
    <li>Recall: ... shows the classification of 'low risk' and 'high risk' loans.</li>
</ul>    


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  <ul>
    <li>Accuracy: The accuracy of the re-sampled data is slightly better. The accuracy went from 99.15% to 99.51%, meaning that the model using resampled data was much better at detecting true positives and true negatives.</li>
    <li>Precission: The was no change in precission for the minority class or the majority class.</li>
    <li>In terms of 'recall', the minority class showed improvement from .89 to 1.00, meaning that the resampled data correctly classified a higher percentage of 'high risk' loan.</li>
  </ul>    

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

<ul><b>Answer</b>:
    <li>In summary, the model was improved after the minority class was improved.</li>
    <li>The model after being oversampled (Learning Machine 2) seems to perform better.</li>
    <li>We are trying to increase the recognition of 'High Risk' loans. The Machine Learning 2 does perform this task.</li>
</ul>

If you do not recommend any of the models, please justify your reasoning.
