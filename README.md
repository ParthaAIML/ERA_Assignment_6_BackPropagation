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
*  **`Complete Back Propagation Calculation`**

### Back Propagation


### Sample output
---
*  **Results**


The accuracy of **`99.41`** has been acheived with **`19`** epoch only



![results](https://github.com/ParthaAIML/ERA_Assignment_6/assets/100613266/3f52c70f-1544-4094-9bcb-a9bfea629cc5)


