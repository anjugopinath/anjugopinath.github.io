---

layout: post
author: anju
title:  Neural Network Classifier
description: Neural Network Classifier
categories: [Neural Network Classifier,Jupyter Notebook,Python ]
image: https://en.wikipedia.org/wiki/Polynomial_regression#/media/File:Polyreg_scheffe.svg

---

[Link to Github](https://github.com/anjugopinath/CS545/blob/main/Gopinath-A4.ipynb)

 NeuralNetworkClassifier

Starting with the NeuralNetwork class defined in Lecture Notes 12, complete the subclass NeuralNetworkClassifier as discussed.
percent_correct

When trying to classify real data, we need a way to evaluate our performance. One way is to just calculate the percent of samples
correctly classified, and to show a confusion matrix. Define the function percent_correct(Y, T), that returns the percent of samples 
correctly classified, given T as a column matrix of class labels, and Y as the column matrix of classes predicted by use.


Apply NeuralNetworkClassifier to Images of Handwritten Digits

Define train_for_best_validation and apply to MNIST data

Using the function run from Lecture Notes 11 as a guide, define a new function train_for_best_validation that accepts arguments

    Xtrain, Ttrain: matrices of shapes $N\times D$ and $N\times 1$ as input and target training data, where $N$ is number of training samples and $D$ is number of input components,
    Xval, Tval: matrices of shapes $N\times D$ and $N\times 1$ of validation data ($N$ not same value as above)
    n_epochs: total number of epochs to train for,
    n_epochs_per_train: divide n_epochs by this value to get number of times the neural network train function is called for this many epochs,
    n_hiddens_list: structure of hidden layers,
    method: optimizer method,
    learning_rate: used for optimizer methods 'adam' and 'sgd'.

It must return

    nnet: resulting neural network with weights that produced the highest accuracy for the validation data set,
    epoch: epoch corresponding to best validation accuracy,
    train_accuracy: accuracy at that best epoch on training data,
    val_accuracy: accuracy at that best epoch on validation data.

This function should call your percent_correct function to calculate classification accuracies.


EXPERIMENT function

This function calls the 'train_for_best_validation' function. It iterates over the list of all parameter variations and calls the 'train_for_best_validation' function. Finally it returns a dataframe table which is displayed.

---

