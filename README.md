# MachineLearning-Homework
### RESAMPLING

#### PROCESS:
1. Created columns for data in csv file.
2. Loaded data from LoanStats csv file.
3. Cleaned data.
4. Encoded dates as integers using LabelEncoder from sklearn.
5. Encoded string data as binary data using get_dummies.
6. Split data Training and Testing.
7. Scaled the training and testing data using StandardScaler from sklearn.
8. Naive Random Oversampling:
    a. Implemented random oversampling with RandomOverSampler from imblearn.
    b. Trained the logistic regression model with LogisticRegression from sklearn.linear_model
    c. Fit the model using the resampled X and y data.
    d. Displayed the Confusion Matrix using confusion_matrix from sklearn.metrics
    e. Calculated the balanced accuracy score using balanced_accuracy_score from sklearn.metrics
    f. Printed the imbalanced classification report using classification_report_imbalanced from imblearn.metrics
9. SMOTE Oversampling:
    a. Resampled the training data using fit_resample and SMOTE from imblearn.over_sampling.
    b. Trained the Logistic Regression model with LogisticRegression from sklearn.linear_model
    c. Fit the model using the resampled X and y data. 
    d. Displayed the confusion matrix
    e. Calculated the balanced accuracy score
    f. Printed the imbalanced classification report
10. Undersampling with Cluster Centroids:
    a. Resampled the training data using fit_resample and ClusterCentroids from imblearn.under_sampling.
    b. Trained the Logisti Regression model
    c. Fit the model using the resampled X and y data.
    d. Displayed the confusion matrix for the test adn prediction data
    e. Calculated the balanced accuracy score for the test and prediction data
    f. Printed the imbalanced classification report for the test and prediction data
11. Combination (Over and Under) Sampling with SMOTEENN
    a. Resampled the training data using fit_resample and SMOTEENN from imblearn.combine
    b. Trained the Logistic Regression model
    c. Fit the model using the resampled X and y data.
    d. Displayed the confusion matrix for the test and prediction data
    e. Calculated the balanced accuracy score for the test and prediction data
    f. Printed the imbalanced classification report for the test and prediction data.
12. FINDINGS:
#### Which model had the best balanced accuracy score?
The Combination (Over and Under) Sampling with SMOTEENN Model

#### Which model had the best recall score?
The Naive Random Oversampling Model


#### Which model had the best geometric mean score?
The Combination (Over and Under) Sampling with SMOTEENN Model


### ENSEMBLE

#### PROCESS:
1. Created columns for the data in the csv file
2. Loaded data from the LoanStats csv file
3. Cleaned data
4. Encoded dates as integers using LabelEncoder from sklearn.preprocessing
5. Encoded string data as binary data using get_dummies
6. Split data into Training and Testing
7. Scaled the training and testing data using StandardScaler from sklearn.preprocessing
8. Balanced Random Forest Classifier
    a. Created the balanced random forest model using BalancedRandomForestClassifier from imblearn.ensemble
    b. Fit the model using the scaled X training data and the y training data
    c. Made predictions using the scaled X testing data
    d. Displayed the confusin matrix as a DataFrame 
    e. Calculated the balanced accuracy score
    f. Printed the imbalanced classification report for the y testing and prediction data
    g. Calculated feature importance using feature_importances_
    h. Sorted features by their importance and displayed as a list
9. Easy Ensemble Classifier
    a. Created the Easy Ensemble Classifier model using EasyEnsembleClassifier from imblearn.ensemble
    b. Fit the model using the scaled X training data and the y training data
    c. Made predictions using the scaled X testing data
    d. Displayed the confusion matrix as a DataFrame for the y testing and prediction data
    e. Calculated the balanced accuracy score for the y testing and prediction data
    f. Printed the imbalanced classification report for the y testing and prediction data
10. FINDINGS:
#### Which model had the best balanced accuracy score?
The Easy Ensemble Classifier Model

#### Which model had the best recall score?
The Easy Ensemble Classifier Model

#### Which model had the best geometric mean score?
The Easy Ensemble Classifier Model

#### What are the top three features?
1 total_rec_prncp, 
2 last_pymnt_amnt, 
3 total_rec_int


