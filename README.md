# Pitch Result Prediction

This jupyter notebook aims to accurately model the result of a pitch given the features "pitcher","batter","zone","p_throws","launch_speed","launch_angle","release_spin_rate","release_speed","release_pos_x", "release_pos_z", "hit_location", "plate_x" and "plate_z".

The predictor is "Description", which is a categorical feature with 14 possible labels. 

We initially choose to use a Random Forest Classifier, given our intuition that the decision boundary between each class is nonlinear. We need to do more EDA to determine whether or not that was a wise choice.

We could potentially use some sort of stepwise feature selection for our model, but we want to get an intuition for how the predictors are related and and choose a decent model initially.

Our initial testing with the full feature set gives us an accuracy score of 71%.

UPDATE 1: Our model improved to a Precision Average of 0.87, Accuracy Score of 0.82 and f1-Score of 0.84

UPDATE 2: Our model after RandomizedSearchCV improved to a Precision Average of 0.89. All other metrics remain the same.
