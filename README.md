# EMNIST Handwritten Digit Classification Three Ways

## Instructions to run the code

* Download the training and test sets from the Kaggle website and put them in the 'data' directory without renaming the files

* Run the PreProcessing.ipynb file in jupyter notebook
	* This will create the final preprocessed data files used in subsequent .ipynb files (both for the training and test data)
	* This file will also create intermediate data files such as "bw_rescaled_x.csv" which contains all of the images with black background and white digits with the largest digit extracted (~96% accuracte extraction of the largest digit)

* Run any of the LogisticRegression.ipynb, NeuralNet.ipynb, and ConvNet.ipynb files in jupyter notebook
	* You should be able to press play in the jupyter notebook and have the code run
	* Each program prints the performance on the validation set and the LogisitcRegression.ipynb and ConvNet.ipynb files produce predicts for the processed test dataset
	* Predictions are stored in either "data/LogisitcPredictions.csv" or "data/ConvNetPrediction#.csv" where # is either nothing, 2, or 3

-----------------------
Check out [this report](https://docs.google.com/document/d/1mtDkIJKRnIvzvoUacq2aG6XGfabagbM0i5N6rloQO1Q/edit) outlining the work in this repo.
