# ERA_Assignment_6


![era](https://github.com/ParthaAIML/ERA_Assignment_5/assets/100613266/71a005f6-ce58-42c9-96f8-4d0954db54bd)
---

## Table of contents
---
* [General info](#general-info)
* [Setup](#setup)
* [Files info](#files-ino)
* [Model info](#model-ino)
* [Execution info](#execution-info)
* [Sample output](#sample-output)

### General info
---
`This repository contains the ipython notebook named as S6-Assignment-Solution used for the assignment 6 of the ERA course. Here we have build a CNN model to predict the hand written digits [0-9] using MNIST data availabe with torchvision library. The objective of this assignment is to create a CNN model(network) which can achive validation accuracy >=99.40 % under few constarints, the constraints are mentioned below`

* The model should acheive 99.4% validation accuracy
* The model should have less than equal to 20k parameters
* The model should achive this accuracy with less than 20 epochs  

`The below points are good to have but not mendatory`

### Setup
---
The below requirements needs to be installed before running the code

#### Requirements
* `torch`
* `torchvision`
* `torchsummary`

### Files info
---
There is one ipython notebook inside the S6 folder in this repository, the name of the notebook is.
*  **`S6-Assignment-Solution.ipynb`**


The **`S6-Assignment-Solution.ipynb`** is a ipython notebook contains all the code to run and validate the model.

### Model info

The details of the `CNN Model(network)` is given below.

The input to the model is a `28x28x1` black and white image containing the digits from `0-9`

The first CNN block has 16 channels of size `3x3`, the convolution are done with padding of 1 to make sure the output size is same as input

The second CNN block has 32 channels of size `3x3`, the convolution are done with padding of 1 to make sure the output size is same as input

Then max pooling is applied to the output to reduce the size of the output image

The third CNN block has  10 channels of size `3x3`, the convolution are done with padding of 1 to make sure the output size is same as input followed by a max pooling

The output of this convolution block is flattened and passed through fully connected layers one containing 20 hidden neurons and the last one contains 10 which is equal o the size of the output

Relu activation is used followed by batch normalization. The details of the network is given below

Total number of parameters used is **`17,920`** 

 
The training of the model is done with **`Stochastic Gradient Descent Optimizer(SGD)`** with a learning rate of **`0.01`** and momentum of **`0.85`**. The batch size used here is **`128`**

 
 ![model_summary](https://github.com/ParthaAIML/ERA_Assignment_6/assets/100613266/e0386845-d481-463b-9364-87078abe6f04)

 
### Execution info
---
The repository can be cloned using the below git command

`git clone https://github.com/ParthaAIML/ERA_Assignment_6`

The user needs to run the **`S6-Assignment-Solution.ipynb`** notebook to get the desired output


### Sample output
---
*  **Results**


The accuracy of **`99.41`** has been acheived with **`19`** epoch only



![results](https://github.com/ParthaAIML/ERA_Assignment_6/assets/100613266/3f52c70f-1544-4094-9bcb-a9bfea629cc5)


