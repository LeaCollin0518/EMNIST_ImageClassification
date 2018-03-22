# EMNIST Handwritten Digit Classification Three Ways

-----------------------
Check out [this report](https://docs.google.com/document/d/1mtDkIJKRnIvzvoUacq2aG6XGfabagbM0i5N6rloQO1Q/edit) outlining the work in this repo.

## Instructions to run the code

* Load the training and test sets and put them in a subdirectory of wherever you are running the code and call the subdirectory 'data'

* Run the PreProcessing.ipynb file
	* This will create the final preprocessed data files used in subsequent .ipynb files (both for the training and test data)
	* This file will also create intermediate data files such as "bw_rescaled_x.csv" which contains all of the images with black background and white digits with the largest digit extracted (~96% accuracte extraction of the images)

* Run any of the LogisticRegression.ipynb, NeuralNet.ipynb, and ConvNet.ipynb files in jupyter notebook
	* You should be able to press play in the jupyter notebook and have the code run
	* Each program prints the performance on the validation set and the LogisitcRegression.ipynb and ConvNet.ipynb files produce predicts for the processed test dataset
