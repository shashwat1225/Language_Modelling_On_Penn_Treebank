## Penn Treebank Language Model


This repository contains code for creating a language model on the Penn Treebank dataset. The language model is implemented using PyTorch and is trained, validated and tested using the provided code.

# Getting Started

To get started, you will need to install the following dependencies:

PyTorch
Matplotlib
tqdm
datasets (from huggingface)
You can install these dependencies using pip.

Once you have installed the dependencies, you can use the provided code to train, validate and test the language model.

# Data Extraction and Tokenization


The Penn Treebank dataset is loaded and processed using the load_dataset function from the datasets module. This function downloads and prepares the dataset, and returns a DatasetDict object that contains the train, test and validation splits of the dataset.

The length of each sentence in the dataset is plotted using Matplotlib to get an idea of the distribution of sentence lengths.

# Model Definition and Training

The language model is defined using PyTorch and consists of an embedding layer, two LSTM layers and a linear layer. The model is trained using the Adam optimizer and the negative log likelihood loss.

The model is trained for a fixed number of epochs and the training and validation loss is plotted after each epoch to visualize the progress of training.

# Evaluation

Once the model is trained, it is evaluated on the test split of the dataset. The perplexity of the model on the test set is calculated and reported.

Conclusion
The provided code can be used to train, validate and test a language model on the Penn Treebank dataset. The model can be further fine-tuned and improved by experimenting with different hyperparameters and architectures.
