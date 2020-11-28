---

layout: post
author: anju
title:  Neural Network Class
description:  Define a new class named Neural Network that constructs a neural network with any number of hidden layers
categories: [Neural Network Class,Jupyter Notebook,Python ]
image: https://en.wikipedia.org/wiki/Polynomial_regression#/media/File:Polyreg_scheffe.svg

---

[Link to Github](https://github.com/anjugopinath/CS545/blob/main/Gopinath-A3.ipynb)

 

You will define a new class named NeuralNetwork that constructs a neural network with any number of hidden layers. 
To train the neural network, you will use the optimizers.py code.Your class must implement at least the following functions.
Lecture Notes 07 provide examples of some of the code in the section about using Optimizers on which you can base your implementation.

    __init__(self, n_inputs, n_hiddens_list, n_outputs):
    __repr__(self):
    make_weights(self): called from constructor __init__
    initialize_weights(self): called from constructor __init__
    train(self, X, T, n_epochs, learning_rate, method='adam', verbose=True): method can be 'sgd', 'adam', or 'scg'. Must first calculate standarization parameters, stored in stand_params dictionary, and standardize X and T. Import optimizers.py and use these optimizers in this train function. Use the tanh activation function.
    use(self, X, return_hidden_layer_outputs=False): standardizes X then calculates the output of the network by calling forward and unstandardizing the network output. Returns just the output of the last layer. If return_hidden_layer_outputs is True, return two things, the output of the last layer and a list of outputs from each hidden layer.
    get_error_trace(self): just returns the error_trace

 

---

