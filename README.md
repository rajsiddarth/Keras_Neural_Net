# NN_Keras

## Dataset

Diabetes data set is used with target and 8 independent variables.

## Objective

- Build a Neural net model to predict the outcome of the target variable.

- Neural Net is built using Keras.Keras is a high-level neural networks API, written in Python and capable of running on top of TensorFlow, CNTK, or Theano. It was developed with a focus on enabling fast experimentation. Being able to go from idea to result with the least possible delay is key to doing good research.[https://keras.io/]. It Allows for easy and fast prototyping (through user friendliness, modularity, and extensibility).It supports both convolutional networks and recurrent networks, as well as combinations of the two. ItRuns seamlessly on CPU and GPU.

## Building Neural Net in Keras

Models in Keras are defined as a sequence of layers.First sequential model is created and layers are added one at a time. The best network structure is found through a process of trial and error experimentation.For our objective we will build a fully-connected network structure with three layers.
- The first layer has 12 neurons and expects 8 input variables. 
- The second hidden layer has 8 neurons and 
- Finally the output layer has 1 neuron to predict the class
- Tensor flow is not supported in python 3.6.Hence we use Theano backend.

## Compiling model in keras

Before training a model, you need to configure the learning process, which is done via the compile method. It receives three arguments:
- an optimizer     : This could be the string identifier of an existing optimizer (such as rmsprop or adagrad), 
                   or an instance of the Optimizer class.
- a loss function  : This is the objective that the model will try to minimize. It can be the string identifier 
                   of an existing loss function (such as categorical_crossentropy or mse), or 
                   it can be an objective function.
- a list of metrics: For any classification problem you will want to set this to metrics=['accuracy']. 
                   A metric could be the string identifier of an existing metric or a custom metric function.

