---
title: How To Implement A Neural Network From Scratch
date:   2019-05-10
tags:
  - python
  - machine learning
  - deep learning
author_profile: false
excerpt: Basics to a Neural Network Without Python Packages
toc: true
mathjax: true
published: true
---

<img src="neural_network_fibers.jpeg" width="400">


To have a basic understanding of the underlying mechanisms of an Artifical Neural Network model, imagine a neural network as a 
brain. Within oushownr brain there are probably billions of neurons bouncing back and forth sending information to different parts 
of our body. These active neurons are known as synapses and is how we learn things. In a neural network, activation functions 
are super important. They work similar to synapses by helping the model perform better by learning the complex patterns within
the data. Fooedfoward and back propogation algorithms were the processes to train the model. Side note: The artifical neural network model was 
originally developed in 1943 by Warren McCulloch and Walter Pitts. 

##Project Overview:

The architecture of the neural network is a four-layered structure that used data with 5 input features, 2 
hidden layers, and 2 output features. Weights and Bias were randomly selected. Feed-forward and back propogation algorithms 
were utilized. Sigmoid and ReLu (Rectified Linear Unit) activation functions were tested and gradient descent employed to 
optimize the sum of square residual (SSR) value. This artifical neural network has been trained and tested data without the help of built-in Python 
packages.

<img src="Network_structure.png" width="400">

Image: Multi-layer Artificial Neural Network Structure

##Code in review:

Feed-forward process: This multi-layer neural network accepts five input values, which we will call features of the training 
data. These featuresshown were multiplied by corresponding "weights" and the products are added to the bias.(input features x weights) + "bias" is computed and is passed into the each layer, which contains specific activation functions. These activation functions produces the final output. The output of the current layer will be the input to the next layer and then it repeats. Code shown below:

<img src="network_size.png" width="400">

<img src="feedforward_intializing.png" width="400">

#Activation functions

<img src="activation_function.png" width="400">

#Feed-Forward 
<img src="forward_feed.png" width="400">

#Back Propagation/
Back Propagation tries to find the error from the output found in the feed-forward by using the weights, loss function, and 
gradient decents.With the right learning rate and additional epochs (cycles), hopefully the algorithms is able to find the a 
better minimun as it moves throughout the gradient decent. The loss function allows for measuring how well the network is 
performing.

<img src="learningrate_lossfunction.png" width="400">

<img src="back_proprogation.png" width="400">

#Results:  
Overall, the Sigmoid function is not as good as the ReLU activation function in this case because ReLU provided 
more accurate predictions. With learning rates and increasing epochs being identical, ReLU continued to improve at a quicker 
rate over Sigmond. 

Image: Learning Improved when SSR Value Decreased

<img src="NNSigmoid.png" width="400">

<img src="NNReLu.png" width="400">
 
