# BUILDING YOUR FIRST NEURAL NETWORK
Modern era is data driven. Data and information are being collected and stored more than we can process. Dealing with such copious amount of data requires speed, accuracy and utmost efficacy. The conventional method of dealing with such an abundance of information is highly inefficient and inaccurate. This issue engendered an approach that is robust, diligent, accurate and highly reliable. Deep learning plays a crucial role in today’s fast-paced technological era. It is versatile and is being utilized in almost every field. The applications of deep learning have proliferated in the past decade. From image recognition to financial management, it has proven to be an essential tool for modern technology. It has ameliorated the quotidian life of a common man.

A neural network is essentially a mathematical function that formulates an output, based on a given input. It mimics the functionality of the human brain. Our network primarily performs tasks and produces accurate predictions by analyzing previously acquired training data. Before we tear into the code, let us get acquainted to some terminologies and key concepts.

## NETWORK ARCHITECTUTE 
A neural network typically consists of:

1) AN INPUT LAYER: Initial dataset which is fed to our model.

2) HIDDEN LAYERS: An arbitrary number of layers between the input and output layers.

3) OUTPUT LAYER: Computes a value which essentially is the prediction of a given input.

## SINGLE NEURON
It is the basic unit of a neural network. It is often referred to as a node. It is connected to nodes from the previous layer, and is associated with a weight (w), bias (b) and an input. A typical node performs a mathematical operation on the weighted sum of its input and formulates an output that is passed onto the next layer.

## ACTIVATION FUNCTION
The operation performed on the weighted sum is a mathematical function referred to as the activation function. The activation function decides if the node is activated or not. It is used to introduce non-linearity into each node’s output. Neural networks incorporate a wide range of activation functions and depends on the application. To name a few:
1) RELU 2) SIGMOID 3) TANH

The aforementioned bias (b) is used to introduce a constant to every node, which plays a role in shifting the activation function to the right or left.

## TRAINING 
Training process involves the following steps:

1.Initialize weights: All weights and biases in the network are assigned random weights with the help of numpy. Note that it is a good practice to be aware of the dimensions of input, weights, biases and the output, as this will be helpful in debugging math errors that emerge out of erroneous matrix multiplication.

2.Forward propagation: Ever node calculated the weighted sum of its input and formulates an output which is passed through an activation function.

Z1 = W1*X1 + W2*X2 + W3*X3 + b1

a1 = g(W1*X1 + W2*X2 + W3*X3 + b1) = g(Z1)

g(z) is an activation function. 

3.BACK PROPAGATION:

COST FUNCTION- It is the difference between the predicted value('h' or 'layer_2') and the actual value('y'). It is a measure our how wrong our model is when juxtaposed with the actual ‘y’ value. Learning rate is a tuning parameter in an optimization algorithm that determines the step size at each iteration while moving toward a minimum of a loss function.

Backpropagation is about understanding how changing the weights and biases in a network changes the cost function. Ultimately, this means computing the partial derivatives dw and db. But to compute those, we first introduce an intermediate quantity, delta_1 and delta_2, which we call the error in the lth layer. Backpropagation will give us a procedure to compute the error delta, and then will relate delta to dw and db. For detailed info about back propagation I highly recommend you to go through this article We repeat this process with all other training examples in our dataset. Then, our network is said to have learnt those examples.

## CONCLUSION
As you can see the predicted value is very accurate. Using algorithms, neural networks can recognize hidden patterns and correlations in raw data, cluster and classify it, and – over time – continuously learn and improve.This article helps us build an intuition for the network. Complex mathematical formulations and derivations are avoided. For additional information I highly recommend going through the references.



