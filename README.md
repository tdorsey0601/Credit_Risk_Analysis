# Credit_Risk_Analysis
module 18

Overview of the analysis:
In this project we are taking a look at how all the factors in our loan_stats csv help predict whether someone is low or high risk status. One method that data scientists use for this type of issue is creating a model and then evaluate and train the models that they create. In this specific project we are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first couple of models we oversampled the data using random over sampler and smote algorithms and under sample the data with the clustercentroid algorithm. In the remaining models we used a combination approach to over and under sample the data using smoteenn. Finally, we compared two machine learning models that minimize bias, balanced random forest classifier and easy ensemble classifier.

Naive Random Oversampling results: Our balanced accuracy test it 65%, the precision for the high_risk has a very low positivity at 1% and the recall is 71%
 ![image](https://user-images.githubusercontent.com/111245707/210110556-d598b075-ee0d-453b-ba9f-e7418d85f9a8.png)


SMOTE oversampling results: the accuracy score is 66%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall smote
 ![image](https://user-images.githubusercontent.com/111245707/210110575-fa46558a-d828-4183-832b-79b6af448074.png)


Undersampling results: balanced accuracy score is about 66% overall, the precision is at 99% and the recall is 40% undersampling
 ![image](https://user-images.githubusercontent.com/111245707/210110587-aacedae7-f53d-46e8-b564-77978afe4ef4.png)


Combination(over and undersampling) results: balanced accuracy score is about 54% the precision is 99% and the recall is 57% overall combination
 ![image](https://user-images.githubusercontent.com/111245707/210110597-1d47ac72-80de-48f4-a584-81a7b290fbf2.png)



Balanced Random Forest Classifier results: the accuracy score is about 78% the precision is 99% and the recall is 88% random forest
 ![image](https://user-images.githubusercontent.com/111245707/210110604-79c01b19-424c-4a36-8d45-5ddbc4925c15.png)


Easy Ensemble AdaBoost Classifier results: the accuracy score is about 91% the precision is 99% and the recall is 94% ensemble
 ![image](https://user-images.githubusercontent.com/111245707/210110609-0a246f06-2d81-4374-b7df-d665089a19dc.png)


Summary:
In the first four we under sampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. We typically want a good balance of recall and precision which is why a recommendation of using the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of its high accuracy score and good balance of precision and recall scores.

