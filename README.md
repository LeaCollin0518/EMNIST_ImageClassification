# EMNIST Handwritten Digit Classification Three Ways

## Brief Outline of Repo Contents

This repo contains code related to [this kaggle competition](https://www.kaggle.com/c/comp551w18-modified-mnist).

This repo contains exclusively data and `.ipynb` files for processing, training, and predicting on that data.  Specifically, there is:

* The `data` folder.  This is where all the data is meant to be.
* `PreProcessing.ipynb`, which contains code that takes the initial dataset and produces a dataset that is ready to be fed to the learning algorithms in this repo.
* `ConvNet.ipynb`, which contains the code for loading data and running a few different Keras CNNs.
* `LogisticRegression.ipynb`, same but for sklearn Logistic Regression.
* `NeuralNet.ipynb`, same but for a 'written-by-hand' implementation of a vanilla NeuralNetwork using Numpy.

## Instructions to run the code

1. Download the training and test sets from the Kaggle website and put them in the 'data' directory without renaming the files

2. Run the PreProcessing.ipynb file in jupyter notebook
	* This will create the final preprocessed data files used in subsequent `.ipynb` files (both for the training and test data)
	* This file will also create intermediate data files such as `bw_rescaled_x.csv` which contains all of the images with black background and white digits with the largest digit extracted (~96% accurate extraction of the largest digit)

3. Run any of the `LogisticRegression.ipynb`, `NeuralNet.ipynb`, and `ConvNet.ipynb` files in jupyter notebook
	* You should be able to press play in the jupyter notebook and have the code run
	* Each program prints the performance on the validation set and the `LogisitcRegression.ipynb` and `ConvNet.ipynb` files produce predicts for the processed test dataset
	* Predictions are stored in `data/LogisitcPredictions.csv`, `data/ConvNetPrediction.csv`, `data/ConvNetPrediction2.csv`, and `data/ConvNetPrediction3.csv` (3 ConvNets were used for predicting on the test set)

-----------------------
Check out [this report](https://docs.google.com/document/d/1mtDkIJKRnIvzvoUacq2aG6XGfabagbM0i5N6rloQO1Q/edit?usp=sharing) outlining the work in this repo.
