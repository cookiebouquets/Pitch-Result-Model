# Pitch Result Prediction

This jupyter notebook aims to accurately model the result of a pitch given the features "pitcher","batter","zone","p_throws","launch_speed","launch_angle","release_spin_rate","release_speed","release_pos_x",and "release_pos_z".

The predictor is "Description", which is a categorical feature with 14 possible labels. 

We initially choose to use a Random Forest Classifier, given our intuition that the decision boundary between each class is nonlinear. We need to do more EDA to determine whether or not that was a wise choice.

We could potentially use some sort of stepwise feature selection for our model, but we want to get an intuition for how the predictors are related and and choose a decent model initially.

Our initial testing with the full feature set gives us an accuracy score of 71%.

TODO:
  1. Run PCA as a dimension reduction technique and rerun the classifier with the PCs as our predictors
  2. Try other classification methods, i.e. Logistic Regression, SVM, KNN, etc. to see if we get a better accuracy score.
  3. Try other CV methods, such as K-fold CV.
