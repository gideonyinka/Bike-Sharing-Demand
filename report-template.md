# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE
YINKA OKUNOLA
## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: I realised that I had to remove any negatives values and replaced them with zero. The changes needed were replacement of negative values with zeros.

### What was the top ranked model that performed?
TODO: The top ranked model was *WeightedEnsemble_L3*

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: It found out the features that needs data wrangling such as datetime and transformed them into new individual features of years, months, and days. It also converted integer datatype of season and weather into category. 

### How much better did your model preform after adding additional features and why do you think that is?
TODO: My model performed better because the score value increased and kaggle score improved. This is because the models were exposed to more features and the models were able to recognise the features "season" and "weather" as category instead of initial interger datatypes.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: The model performed better when I changed the eval_metric to "r2" unlike "root-mean-squared-error" and increase the time_limit. However, the score value decreased when I changed the hyperparameters from default to light and very_light, and also when I tried to change the hyperparameters of of NN and GBM. I also noticed there was drop in score value when presets was changed to "best_quality_with_high_quality_fit".

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: I will like to increase the time_limit more, add more new features to the data, and selectively focus on "WeightedEnsemble_L3" model to tune the hyperparamaters.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|eval_metric|presets|time_limit|1.80496|
|add_features|eval_metric|presets|time_limit|1.78022|
|hpo|eval_metric|presets|time_limit|1.77960|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: The top model with high score value was *WeightedEnsemble_L3*. The  model prediction improved as more new features were added and tune the hyperparameters most especially the time_limit and eval_metric.

```
Kaggle_username = "yinklagabriel"
kaggle_password = "61a4f22e232bd17244ba77c247cc1212"

```

