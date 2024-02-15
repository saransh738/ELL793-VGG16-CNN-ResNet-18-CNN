# VGG-16 Convolution Neural Network
## Problem Statement:
* Train VGG-16 CNN from scratch using the MNIST dataset (which contains images of
handwritten digits categorized into classes of 0 to 9)
* (Which Activation function is better?) Fix the number of epochs (to 50 epochs) and fix any learning rate, optimizer, or batch size, and train this network, with layers having:
  - only RELU activation,
  - only leaky RELU activation,
  - only sigmoid activation,
  - only tanh activation.
We need to produce the type of class using Softmax after the last layer, in all the
above cases. Tabulate/Plot and discuss the convergence of the network upon these
different activations.
* (What learning rate is better?) Fix the optimizer, batch size, and activation function, the number of epochs (to 50 epochs), and train this network first using different learning rates (of your choice). Tabulate/Plot and discuss the convergence of the network upon varying learning rates.
* (Role of optimizer) Fix the number of epochs, learning rate, batch size, and activation function, train this network first using the following optimizers:
  - Vanilla Gradient descent
  - Momentum-based gradient descent (momentum value of your choice)
  - Adam.
  - RMS prop.
Tabulate/Plot and discuss the convergence of the network upon using these different optimizers.
* (Transfer Learning) So far, we have understood the best/optimal hyperparameters that yield the best performance in your set of experiments. Save the weights/configuration of this model (this is what we will call the pre-trained model). In this experiment, rather than classifying the images into classes 0 to 9, we will slightly change the problem statement in the following way:
  - The dataset with digits 0-9 has mainly two types of information: either the handwritten digit is made using a curved stroke or a straight stroke (or maybe both). Hence, divide the dataset into two classes viz., the set of digits with curved stroke(s) C: {0,2,3,5,6,8,9} and the set of digits with straight stroke(s), S: {1,4,7}.
  - Modify the last layer of the network so that now it can classify the digit into class ‘C’ or class ‘S’. Initialize the network with the weights of the pre-trained model (except the weights of the penultimate layer that must be trained). In other words, retrain only the last layer of the network keeping the weight of all other layers the same as were in the pre-trained model.
Use the optimal hyperparameters (of your choice). Tabulate/Plot and discuss the convergence of the network in this task of transfer learning.

# ResNet-18 Convolution Neural Network
## Problem Statement:
* Train a CNN network with ResNet-18 as a backbone from scratch with CIFAR-10 and note down the performance.
*  Initialize the ResNet-18 network with pre-trained weights from ImageNet and then try to use these weights to improve the training for the CIFAR-10 dataset. Try to come up with different ways of using these weights to improve the performance and play with the hyper-parameters to get the best performance. Document the results of your experiments.
* Train the network from scratch with the Tiny-CIFAR-10 dataset. Try using as many data augmentation techniques as you can think of to try to improve the performance.
Try to drop out after different layers and with different dropout rates. Document the results of your experiments.
* Visualize the activations of the CNN for a few test examples in each of the above cases. How is the activation in the first few layers different from the later layers?
* For the Tiny-CIFAR-10 dataset, take 500 images per class from CIFAR-10 for training. Use the same 10,000 images for testing as per the CIFAR-10 dataset.
