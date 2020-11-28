---

layout: post
author: anju
title:  Multilayered Neural Network
description: Multilayered Neural Network to predict continuous-valued target values
categories: [Multilayered Neural Network,Jupyter Notebook,Python ]
image: https://en.wikipedia.org/wiki/Polynomial_regression#/media/File:Polyreg_scheffe.svg

---

[Link to Github](https://github.com/anjugopinath/CS545/blob/main/Gopinath-A2.ipynb)

 Implement a set of functions for training and testing a multilayered neural network to predict continuous-valued target values. 
 This assignment provides an implementation of the functions for a neural network with one hidden layer.
 You must modify the functions to allow any number of hidden layers, each with any number of units.

---

FUNCTION DESCRIPTION:

    add_ones(X): Given an 𝑁×𝐷

matrix of inputs, prepend column of 1's and return the resulting 𝑁×𝐷+1
matrix.
make_weights(n_inputs, n_hiddens, n_outputs): Given integers n_inputs, n_hiddens and n_outputs, create weight matrices V for the hidden layer and W for the output layer.
forward(Xst, V, W): Given standardized input matrix Xst and weight matrices V and W, calculate the output of all layers and return the outputs of the hidden layer, Z as an 𝑁×𝐻
matrix, where 𝐻 is the number of hidden units, and the outputs of the output layer Y as an 𝑁×𝐾 matrix, where 𝐾
is the number of output values for each sample.
backward(Xst, Tst, V, W): Given standardized input matrix Xst, standardized target matrix Tst, and weight matrices V and W,, calculate the gradient of the mean squared error with respect to the weights V and W, returning a tuple of both gradients, with respect to V as the first element and with respect to W as the second element.
train_sgd(X, T, V, W, learning_rate, n_epochs): Given input and target matrices X and T, weight matrices V and W, a learning_rate and the number of epochs to train, update the weights for n_epochs iterations using the gradient of the mean squared over the whole data set in X and T and return the resulting new weight matrices V and W, the standardization parameters, and the list of RMSE training errors, one per epoch.
use(X, V, W, stand_parms): Calculate outputs of both layers after standardizing input X. Return outputs of hidden layer, and unstandardized output of output layer.
rmse(Y, T): Return the RMSE between Y and T, both of which are not standardized.
calc_standardize_parameters(X, T): calculate and return as a dictionary the column means and standard deviations of X and T.
standardize_X(X, stand_parms): return standardized X.
standardize_T(T, stand_parms): return standardized T.
unstandardize_X(Xst, stand_parms): return unstandardized X (probably not needed).
unstandardize_T(Tst, stand_parms): return unstandardized T, will be needed by use.

