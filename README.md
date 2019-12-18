# Kaggle - Titanic

For this competition, I have decided to try an Ensemble Stacking method. 

The base classifiers that I have used are Logistic Regression, Random Forest, AdaBoost, Gradient Boosting, Extra Trees and Support Vector Classifier from sklearn. I have used GridSearchCV for hyper parameter tuning. The probabilities from each classifier have been fed as the training data for the secondary classifier. To get the probabilities of the predictions in the training data, I have used KFold to split the training data and then predicted the probabilities on the fold that wasn't used to train in that particular iteration. The secondary classifier that I used is the XGBoost Classifier. 

I have included implementations of just the base classifiers as well. The ensemble technique has been applied with and without feature engineering.
