# VGG-16 Convolution Neural Network
## Problem Statement:
* Training VGG-16 CNN from scratch using the MNIST dataset (which contains images of
handwritten digits categorized into classes of 0 to 9)
* (Which Activation function is better?) Fixing the number of epochs (to 50 epochs) and fixing any learning rate, optimizer, or batch size, and train this network, with layers having:
  - only RELU activation,
  - only leaky RELU activation,
  - only sigmoid activation,
  - only tanh activation.
We need to produce the type of class using Softmax after the last layer, in all the
above cases. Tabulate/Plot and discuss the convergence of the network upon these
different activations.
* (What learning rate is better?) Fixing the optimizer, batch size, and activation function, the number of epochs (to 50 epochs), train this network first using different learning rates (of your choice). Tabulate/Plot and discuss the convergence of the network upon varying learning rates.
* (Role of optimizer) Fixing the number of epochs, learning rate, batch size, and activation function, train this network first using the following optimizers:
  - Vanilla Gradient descent
  - Momentum-based gradient descent (momentum value of your choice)
  - Adam.
  - RMS prop.
Tabulate/Plot and discuss the convergence of the network upon using these different optimizers.
* (Transfer Learning) So far, we have understood the best/optimal hyperparameters that yield the best performance in your set of experiments. Save the weights/configuration of this model (this is what we will call the pre-trained model). In this experiment, rather than classifying the images into classes 0 to 9, we will slightly change the problem statement in the following way:
  - The dataset with digits 0-9 has mainly two types of information: either the handwritten digit is made using a curved stroke or a straight stroke (or maybe both). Hence, divide the dataset into two classes viz., the set of digits with curved stroke(s) C: {0,2,3,5,6,8,9} and the set of digits with straight stroke(s), S: {1,4,7}.
  - Modify the last layer of the network so that now it can classify the digit into class ‘C’ or class ‘S’. Initialize the network with the weights of the pre-trained model (except the weights of the penultimate layer that must be trained). In other words, retrain only the last layer of the network keeping the weight of all other layers the same as were in the pre-trained model.
Use the optimal hyperparameters (of your choice). Tabulate/Plot and discuss the convergence of the network in this task of transfer learning.
