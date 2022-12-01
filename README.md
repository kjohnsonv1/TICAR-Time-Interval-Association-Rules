# TICAR-Time-Interval-Association-Rules

Two runnable experiments - Embedded Reber Grammar and Titarl99.

# Embedder Reber Grammar

## Mine association rules

Run with:

`java -jar TrainReber.jar`

Learned models (.model) are human readable and will be output to /ReberTrainResults/Batch summary/ExportModels/


## Generate predictions

Run with:

`java -jar TestReber.jar`

Prediction files (.pred) will be generated in ReberTestResults/Predictions/


## Evaluate predictions

The 3rd party evaluation program is provided with the Titarl99 datasets.
Download Titarl datasets from https://mathieu.guillame-bert.com/dataset#computergenerate


Extract dataset zip file to folder.

Copy evaluatePrediction.py from the extracted folder into the ReberDataset folder. This will simplify evaluation because the default folders will be set correclty.

Run evaluatePrediction.py from the ReberDataset folder. It requires python 2.7. For example:

`C:/"Program Files (x86)"/Python27/python evaluatePrediction.py`

- Set "User predictions directory" to the prediction output folder e.g. ReberTestResults/Predictions/
- The remaining directory defaults should be ok with default values, if evaluatePrediction.py is run from the ReberDataset folder.
- Click "Start analyse"


# Titarl99

99 synthetic datasets with varying amounts of noise.  

## Download Titarl99 datasets

Download Titarl datasets from https://mathieu.guillame-bert.com/dataset#computergenerate

Extract dataset zip file to folder.

## Mine association rules

Set titarl99DatasetFolder value in TrainTitarl99.ini to the dataset root folder, e.g. titarl99DatasetFolder=TitarlDatasets/

Run with:

`java -jar TrainTitarl99.jar`

Learned models (.model) are human readable and will be output to /Titarl99TrainResults/Batch summary/ExportMinimalModels/


## Generate predictions

Set titarl99DatasetFolder value in TestTitarl99.ini to the dataset root folder, e.g. titarl99DatasetFolder=TitarlDatasets/

Run with:

`java -jar TestTitarl99.jar`

Prediction files (.pred) will be generated in Titarl99TestResults/Batch summary/Predictions/


## Evaluate predictions

Run evaluatePrediction.py from the Titarl datasets folder. It requires python 2.7. For example:

`C:/"Program Files (x86)"/Python27/python evaluatePrediction.py`

- Set "User predictions directory" to the prediction output folder e.g. Titarl99TestResults/Batch summary/Predictions/
- The remaining directory defaults should be ok with default values, if evaluatePrediction.py is run from the Titarl datasets folder.
- Click "Start analyse"

