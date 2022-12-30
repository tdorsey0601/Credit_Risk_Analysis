# Credit_Risk_Analysis
module 18

Overview of the analysis:
In this project we are taking a look at how all the factors in our loan_stats csv help predict whether someone is low or high risk status. One method that data scientists use for this type of issue is creating a model and then evaluate and train the models that they create. In this specific project we are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first couple of models we oversampled the data using random over sampler and smote algorithms and under sample the data with the clustercentroid algorithm. In the remaining models we used a combination approach to over and under sample the data using smoteenn. Finally, we compared two machine learning models that minimize bias, balanced random forest classifier and easy ensemble classifier.

