# machine-learning-challenge

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system. The [Exoplanet Data](Models/exoplanet_data.csv) has various observations for the planets. We have used following supervised learning models to train the data:

* [Decision Tree](Models/model_1.ipynb)

* [Random Forest](Models/model_2.ipynb)

## Decision Tree

With this model, training score for the model was 1.0 while the test score was around 0.85. This training score is very high so it indicates the overfitting tendency of Decision Trees. This model predicts Confirmed exoplanets better than False Positive, however has very low score for Candidate. Excluding bottom 5 features with the lowest weight doesn't have much impact on the score.

## Random Forest

This model has overall better score for Test and Train data. The grid search indicates that the n_estimators should be around 40 with an scroe of 0.89. Excluding bottom 5 features with the lowest weight gets very high accuracy on Candidate category.  

Overall Random Forest modedol does well for predicting exoplanets data.