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

1.Input virtual Layer-: This layer is used to fed 784 pixels to our first hidden Layer of 256 activation functions
   
2. First Hidden Layer-: This is first hidden layer with 256 activation functions  in which each activation fn recieves the 784 values 
                        that is pixels along with a bias and we have used here Relu activation fn .I will explain that after this.
                        Also in this we have 256 bias for each activation fn .

3.Second Hidden Layer-:This is first hidden layer with 256 activation functions  in which each activation fn recieves the 256 values 
                        that is pixels along with a bias and we have used here Relu activation fn .I will explain that after this .
                        In this again we have 256 bias for each activation fn .
                       
4. Output Layer      -: This is final layer which have 10 units that specify each class   
                        
                            
