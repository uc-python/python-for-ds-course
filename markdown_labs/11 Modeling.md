# Modeling – Lab
*Python for Data Science*

1. Build a model using the flights data to predict departure delay. Remember to split your data, examine your data, select features, choose some models to try, train the models, and choose one (possibly based on scoring the models).
    - Be careful to avoid leakage! Make sure all of your features make sense as predictors.
    - Think: do you need a classification or regression model?
        - Some regression models: Linear Regression, Lasso Regression, Decision Tree Regressor, Random Forest Regressor
        - Some classification models: Gaussian Naive Bayes, Decision Tree Classifier, Random Forest Classifier
    - You will find that our features include some categorical variables. We did not cover how to deal with categorical (non-numeric) variables in class. You may either A) drop these features or B) if you're feeling ambitious, look into a technique like one-hot encoding. Try `pd.get_dummies`.
