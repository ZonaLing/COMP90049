# The Correlation Between Movie Rating and Movie Gerne 

## Main Source File
Evaluation_pipeline.ipynb (Please run in Jupyter Notebook.)

## Technical Requirements

The python version is 3.10.2, the code file should be run from top to bottom to obtain all results successfully.

## Project Architecture
The order of the models is the baseline model: logistic regression, then the 2 other training models: decision tree and random forest. 

The results of models can be found on cell [9] and [11] for logistic regression, cell [14] and [17] for decision tree, and cell [27] and [30] for random forest, while the former is the training result with genre data, the later is the training result without genre data.

## Source Data Requirements
### Data files required to run all codes:

The source of data is extracted from the TMDB database.
1. TMDB_train.csv
This dataset is for training machine learning models.
2. TMDB_eval.csv
This dataset is for evaluating machine learning models.
3. TMDB_test.csv
This unlabeled dataset is for testing whether the machine learning models can predict "rate_category" accurately.
4. train_concat_tfidf.npz
This file contains all vectorized data for "title", "overview", "tagline", and "production_companies" features in the training dataset.
5. eval_concat_tfidf.npz
This file contains all vectorized data for "title", "overview", "tagline", and "production_companies" features in the evaluation dataset.
6. test_concat_tfidf.npz
This file contains all vectorized data for "title", "overview", "tagline", and "production_companies" features in the testing dataset.

### The Kaggle files after making predictions on test file using different models:
1. dt_prediction_with_genre.csv
2. dt_prediction_without_genre.csv
3. rfc_prediction_with_genre.csv
4. rfc_prediction_without_genre.csv

