# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Add your explanation
i tried to delete negative values and round the values of the 'count' column

### What was the top ranked model that performed?
TODO: Add your explanation
the WeightedEnsemble_L3 model

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: Add your explanation
it finds that there are columns that are categorical and are relevant for the predictons

### How much better did your model preform after adding additional features and why do you think that is?
TODO: Add your explanation
after adding some features, the model performed well since its performance has increased from -53.126251 to -30.276309 

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: Add your explanation
after trying to tune the model hyperparameters, the kaggle score improved from 0.70217 to 1.79461 

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: Add your explanation
i will try more hyperparameters that will tune my model in a best way

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default|default|default|1.79461|
|add_features|default|default|default|0.70217|
|hpo|CAT(iterations),RF(n_estimators), XT(n_estimators)|GB(num_boost_round, num_leaves)|scheduler, searcher|0.45257|


### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation

i have learned in this project very important things and practices since we began by importing the kaggle dataset about bike sharing demand and we had to do a model that will help us to predict the number of bike demands in terms of different aspects wheter it  was datetime, season, locations or temperature... and we used the autogluon framework that lets ur to choose which model will perform better in our case and we found that the WeightedEnsemble_L3 is the best one even with hyperparameters tuning.