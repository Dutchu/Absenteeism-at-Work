# Data Analysis of: Absenteeism at work
## Source: https://archive.ics.uci.edu/dataset/445/absenteeism+at+work
## Create env

    $ conda env create -f environment.yml
                                                                                                                                                                                                                                                                                 
## To activate this environment, use
                                                                                                                                                                                                                                                                                 
     $ conda activate absent
                                                                                                                                                                                                                                                                                 
## To deactivate an active environment, use
                                                                                                                                                                                                                                                                                 
     $ conda deactivate                                                                                                                                                                                                                                                          


Explanation:
Prepare the Data:

One-hot encoding is applied to convert categorical variables into numerical ones. The drop_first=True parameter avoids multicollinearity by dropping the first column of the encoded result.
Split the Data:

The dataset is split into training (70%) and test (30%) sets to evaluate the model's performance on unseen data.
Train the Model:

A Logistic Regression model is used to train on the training data (X_train and y_train).
Evaluate the Model:

The model's predictions are evaluated using common classification metrics, like precision, recall, F1-score, and confusion matrix.
Next Steps:
Try More Models: Experiment with more complex models like Decision Trees, Random Forests, or Gradient Boosting.
Feature Engineering: Create new features that might help the model, such as combining existing features or creating new derived features.
Hyperparameter Tuning: Use techniques like Grid Search or Randomized Search to find the best hyperparameters for your model.
Deploy the Model: Once satisfied with the model's performance, you can deploy it for use on new data.