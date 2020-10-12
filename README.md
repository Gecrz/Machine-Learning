# Machine-Learning

In this project we will build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so we will need to employ different techniques for training and evaluating models with imbalanced classes. We will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. [Resampling](#Resampling)
2. [Ensemble Learning](#Ensemble-Learning)

#### Resampling

## Step by step process

1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2. Oversample the data using the `Naive Random Oversampler` and `SMOTE` algorithms.
3. Undersample the data using the `Cluster Centroids` algorithm.
4. Over- and under-sample using a combination `SMOTEENN` algorithm.

For each of the above, you will need to:

1. Train a `logistic regression classifier` from `sklearn.linear_model` using the resampled data.
2. Calculate the `balanced accuracy score` from `sklearn.metrics`.
3. Calculate the `confusion matrix` from `sklearn.metrics`.
4. Print the `imbalanced classification report` from `imblearn.metrics`.

Use the above to answer the following:

> Which model had the best balanced accuracy score?
>
> Which model had the best recall score?
>
> Which model had the best geometric mean score?

#### Ensemble Learning

# Step by step process

Be sure to complete the following steps for each model:

1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2. Train the model using the quarterly data from LendingClub provided in the `Resource` folder.
3. Calculate the balanced accuracy score from `sklearn.metrics`.
4. Print the confusion matrix from `sklearn.metrics`.
5. Generate a classification report using the `imbalanced_classification_report` from imbalanced learn.
6. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.

Use the above to answer the following:

> Which model had the best balanced accuracy score?
>
> Which model had the best recall score?
>
> Which model had the best geometric mean score?
>
> What are the top three features?

### Results

The credit risk ensemble activity, the objective was to analyze two methods: Balanced Random Forest Classifier and Esay Ensemble Classifier. This last one had grea average precision and recall scores at 0.99 and 1.00, low risks scores were better than high risks, meaning that the model is not good at predicting or assessing high risk credit applicants. Meanwhile, the Balanced random forecast classifier did a little better in recall when trying to predit high risk credit applicants. In a situation where a false negative is a huge concern, balanced random forecast classifier method is a better choice. Random forecast had better gemetric mean score and easy and better overall recall, while easy ensemble classifier had a better precision score.

The goal of the other activity was to analyze among all resampling methods: Random Oversampling, Smote oversampling, undersampling and combination sampling, which one performed better.

Among those three methods:

SMOTE oversampling with 0.5320503523212106 score, is the better accurac score.

Radom Oversampling had the better recall score with avg/total of 0.59.

Undersampling had the best geometric mean score of 0.51.
