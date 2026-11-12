# Credit Score Classification Notebook

This project contains a Jupyter notebook for working with the Kaggle credit score classification dataset and exploring a machine learning workflow for predicting a customer's credit score.

## Project files

- `machine_learning_3.ipynb` — main notebook for downloading the dataset, cleaning the data, and building the analysis pipeline.

## Overview

The notebook demonstrates a practical end-to-end workflow for a credit scoring problem:

- downloading the dataset from Kaggle
- loading the training data into pandas
- inspecting the dataset and checking for invalid or inconsistent values
- handling missing data and impossible ranges
- preparing features for a classification model
- training and evaluating a model to predict `Credit_Score`

## Dataset

The notebook pulls the dataset from the Kaggle repository:

- `parisrohan/credit-score-classification`

It uses the dataset files typically available as:

- `train.csv`
- `test.csv`

This project intentionally does not bundle the raw dataset in the repository; the notebook downloads it when run.

## What the notebook does

From the notebook contents, the workflow includes:

- validating downloaded files
- loading the data with pandas
- examining rows and column values
- correcting unrealistic field values such as:
  - `Age` values below 18 or above 55
  - negative or excessive `Num_Bank_Accounts`
  - excessive `Num_Credit_Card` values
  - unrealistic `Interest_Rate` values
- checking for missing values and inconsistent records
- preparing the dataset for modeling and evaluation

## Requirements

To run the notebook, you will need:

- Python 3.x
- Jupyter Notebook or Google Colab
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Example installation:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Run locally

1. Open the notebook in Jupyter or VS Code.
2. Run the cells in order.
3. If needed, install any missing packages the first time you run the notebook.
4. The notebook will download the Kaggle dataset automatically when executed.

## Notes

- The notebook depends on Kaggle access and the dataset being available to the runtime.
- Kaggle download links may require authentication, so if the notebook is run outside the original environment, you may need to use a valid Kaggle API token.
- This is a learning and exploratory project focused on credit score classification rather than a production-ready deployment.
