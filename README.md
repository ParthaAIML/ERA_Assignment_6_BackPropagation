# ERA_Assignment_6_BackPropagation


![era](https://github.com/ParthaAIML/ERA_Assignment_5/assets/100613266/71a005f6-ce58-42c9-96f8-4d0954db54bd)
---

## Table of contents
---
* [General info](#general-info)
* [Files info](#files-ino)
* [Back Propagation](#back-prop)
* [Sample output](#sample-output)

### General info
---
`This repository contains an excel file for backpropagation calculation.Neural networks are computational models inspired by the structure and function of biological neural networks. They consist of interconnected artificial neurons organized in layers. These networks learn from data by adjusting the weights of the connections between neurons to minimize the difference between predicted and actual outputs. Backpropagation is a key algorithm used to train neural networks. It calculates the gradients of the network's error with respect to its weights, enabling the optimization of the network through gradient descent. By iteratively updating the weights based on these gradients, neural networks can learn complex patterns and make accurate predictions across various domains.`

Backpropagation is a key algorithm used for training neural networks. It involves several steps to compute the gradients of the network's error with respect to its weights, enabling the optimization of the network through gradient descent. Here are the different steps of backpropagation:

**`Forward Propagation`**: During forward propagation, the input data is fed into the neural network, and the activations and outputs of each layer are computed sequentially, moving from the input layer to the output layer.

**`Loss Calculation`**: The output of the neural network is compared to the desired output using a predefined loss function. The loss function quantifies the discrepancy between the predicted output and the actual output.

**`Backward Propagation`** of Errors: In this step, the gradients of the loss with respect to the network's weights are computed. The gradient is a measure of how the loss changes with respect to each weight in the network. The chain rule of calculus is used to calculate these gradients by propagating the errors backward through the layers.

**`Weight Update`**: Once the gradients are computed, the weights of the neural network are updated to minimize the loss. This is typically done using an optimization algorithm such as gradient descent. The weights are adjusted in the opposite direction of the gradients, scaled by a learning rate, to iteratively converge towards a better solution.

**`Iteration`**: The steps of forward propagation, loss calculation, backward propagation, and weight update are repeated iteratively for multiple epochs or until a convergence criterion is met. Each iteration allows the network to refine its weights and improve its performance.

By repeating these steps, backpropagation enables the neural network to learn from data and adjust its weights to make more accurate predictions over time.

### Files info
---
There is one excel file containing all the back propagation calculation in this repository, the name of the excel file is.
*  **`Complete Back Propagation Calculation.xlsx`**

### Back Propagation
---

The given network is below


![neural network](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/35a56ef7-e366-4a26-9f73-c9635b309e77)

In this network we have two inputs and two outputs, one hidden layer. There are eight weights in the network `w1`,`w2`,`w3`,`w4`,`w5`,`w6`,`w7` and `w8`. The first four weights connects the input to the neurons of the hidden layer and the last four weights connects the neurons of the hidden lasyer to the output. 
The predicted output are compared with the actutal output which are `t1` and `t2` and a total error `Error=t1+t2` is computed.

The main objective is to learn the relationship between input and output correctly. To acheive that we need to update the weights so that the total error reduces.

This is done via Back Propagation,Back Propagation helps us to compute the gradients of the loss function with respect to each weight and finally update the weights using the below formula


![gd](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/d0042e97-6eb3-41b9-9724-eb4cc70daaba)

**`Forward Propagation`**

In this example, input `i1` and `i2` is getting multiplied with  weights `w1`,`w2`,`w3`,`w4` to produce the output `h1` and `h2` then `h1` and `h2` goes through the activation function (sigmoid,tanh or relu) to produce the output `a_h1` and `a_h2`. Then again `a_h1` then `a_h2` get multiplied with  weights `w5`,`w6`,`w7` and `w8` to produce the output `o1` and `o2`,again `q1` and `q2` goes through the activation function (sigmoid,tanh or relu) to produce the output `a_o1` and `a_o2`. Then the error is computed using `MSE` ad finally the total error is computed.

**`Back Propagation`**

During back propagation the derivative of the loss with respect to the weights   `w5`,`w6`,`w7` and `w8` are computed and then again the derivative or the gradients of the total loss with respect to the weights `w1`,`w2`,`w3`,`w4` are computed. During the gradinet computation the chain rule is used. Below are the gradient computation.


![weight calculation](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/93b69291-3bb6-4195-99c7-4a56a2fb8a57)


Finally the weights are updated and the forward pass are done to get the prediction.

### Sample output
---

Back propagation with different learning rate `[0.1,0.2,0.8,1,2]` has been performed and the results are shown below

*  **Back Propagation with LR 0.01**


![lr_0 1](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/9cb2463d-90cc-4d31-bfa9-28d285685f54)

*  **Back Propagation with LR 0.02**


![lr_0 2](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/ee05b2f9-f537-49d3-b14a-f3800ba846ae)


*  **Back Propagation with LR 0.05**

![lr_0 5](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/d94d7de9-8b46-451f-b7f6-06a190e48948)


*  **Back Propagation with LR 0.08**

![lr_0 8](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/867a1642-fc66-49c5-9a37-fb37b8145638)


*  **Back Propagation with LR 1.0**

![lr_1](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/8dd2a3b0-d6e4-4bfc-8e5d-aedd3256a1c4)


*  **Back Propagation with LR 2.0**

![lr_2](https://github.com/ParthaAIML/ERA_Assignment_6_BackPropagation/assets/100613266/03e1f242-250a-4f91-be3a-ab58669c9c72)

