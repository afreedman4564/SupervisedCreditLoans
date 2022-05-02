# SupervisedCryptoChallenge

## Import dependencies

## Convert categorical data to numeric and separate the dependent variable
- Use drop to remove outcome from the data set
- Create new dataframe with the outcome/dependent variable

## Identify columns present in the training set and not present in the test set
- create list of columns from the training and test sets
- leverage list comprehension loop through the test set on the training set to id those missing
- introduce the missing column(s) into the test set
- convert the missing column(s') values to 0

## Train the training data with Logistic Regression and Random Forest models
- use unscaled and standard scaling to create 4 options
- calculate the model score for each of the 4 options for the training and test sets

## Prediction:
Random Forest with scaled data will have strongest results due to its:
    - emphasis on feature selection
    - feature weighting changes based on importance
    - random samples of 'leaves' of trees can lead to stronger insight


Impact of scaling will improve accuracy given its easing comparison of values and possibly outliers

## Outcome:

Logistic Regression on scaled data appears strongest. Random Forest, in both unscaled and scaled, appears to suffer from overfitting where the score decreases noticeably mobing from training to test. Logistic Regression on scaled data is very consistent from training to test set. Based on this, recommendation is move forward with the Logistic Regression, using scaled data.
