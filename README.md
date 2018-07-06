# Digit-Recognition-using-Tensorflow-and-Neural-Networks
This project performs digit recognition using deep learning concepts. It can classify image into 10 classes.  Here I provide a neural network implementation to perform digit recognition. It implements a simple but efficient  neural network using most popular Google  library tensorflow.

# MNIST database of handwritten digits
The first step is to create a database of handwritten digits. We are not going to create a new database but we will use the popular MNIST database of handwritten digits. The MNIST database is a set of 70000 samples of handwritten digits where each sample consists of a grayscale image of size 28×28. There are a total of 70,000 samples. 

# Prerequisites
* Data Science
* TensorFlow
* Deep Learning
* numpy,sklearn libraries

## The Architecture of Neural Network
### weights & biases

n_input = 784
n_hidden_1 = 256
n_hidden_2 = 256
n_classes = 10

In this i have 4 layers i will explain each one with its specifications

1. Input virtual Layer-: This layer is used to fed 784 pixels to our first hidden Layer of 256 activation functions
   
2. First Hidden Layer-: This is first hidden layer with 256 activation functions  in which each activation fn recieves the 784 values 
                        that is pixels along with a bias and we have used here Relu activation fn .I will explain that after this.
                        Also in this we have 256 bias for each activation fn .

3. Second Hidden Layer-:This is first hidden layer with 256 activation functions  in which each activation fn recieves the 256 values 
                        that is pixels along with a bias and we have used here Relu activation fn .I will explain that after this .
                        In this again we have 256 bias for each activation fn .
                       
4. Output Layer      -: This is final layer which have 10 units that specify each class from 0 to 9 .

## What is Activation Function ?

It’s just a thing (node) that you add to the output end of any neural network. It is also known as Transfer Function. It can also be attached in between two Neural Networks.
Why we use Activation functions with Neural Networks?

It is used to determine the output of neural network like yes or no. It maps the resulting values in between 0 to 1 or -1 to 1 etc. (depending upon the function).

### 1. Sigmoid or Logistic Activation Function


The main reason why we use sigmoid function is because it exists between (0 to 1). Therefore, it is especially used for models where we have to predict the probability as an output.Since probability of anything exists only between the range of 0 and 1, sigmoid is the right choice.

The function is differentiable.That means, we can find the slope of the sigmoid curve at any two points.

The function is monotonic but function’s derivative is not.

The logistic sigmoid function can cause a neural network to get stuck at the training time.

The softmax function is a more generalized logistic activation function which is used for multiclass classification.

### 2. ReLU (Rectified Linear Unit) Activation Function

The ReLU is the most used activation function in the world right now.Since, it is used in almost all the convolutional neural networks or deep learning.


As you can see, the ReLU is half rectified (from bottom). f(z) is zero when z is less than zero and f(z) is equal to z when z is above or equal to zero.

Range: [ 0 to infinity)

The function and its derivative both are monotonic.

But the issue is that all the negative values become zero immediately which decreases the ability of the model to fit or train from the data properly. That means any negative input given to the ReLU activation function turns the value into zero immediately in the graph, which in turns affects the resulting graph by not mapping the negative values appropriately.


                        
                            
