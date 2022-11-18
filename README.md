# TICAR-Time-Interval-Association-Rules

## Download Titarl99 datasets

Download Titarl datasets from https://mathieu.guillame-bert.com/dataset#computergenerate

Extract dataset zip file to folder and set titarl99DatasetFolder value in TrainTitarl99.ini to the dataset root folder, e.g. titarl99DatasetFolder=TitarlDatasets/

## Mine association rules

Run with java -jar TrainTitarl99.jar


## Generate predictions

Set titarl99DatasetFolder value in TestTitarl99.ini to the dataset root folder, e.g. titarl99DatasetFolder=TitarlDatasets/

Run with java -jar TestTitarl99.jar

Prediction files (.pred) will be generated in Titarl99Results\Batch summary\titarlPredictions\


## Evalutate prediction

Run evaluatePrediction.py from the Titarl datasets folder. It requires python 2.7. For example:

C:\"Program Files (x86)"\Python27\python evaluatePrediction.py


# Embedder Reber Grammar

More details to come soon.
