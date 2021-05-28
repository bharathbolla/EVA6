

## Train a Simple Neural Network using Microsoft Excel

### Neural Network Diagram
![image](https://user-images.githubusercontent.com/10822997/120015673-39abe900-c001-11eb-8658-6110395afb4d.png)

![image](https://user-images.githubusercontent.com/10822997/120015690-40d2f700-c001-11eb-8558-912179fda1eb.png)

Draw the neural network diagram as shown in the figure.
Connect all the neurons using arrows and mark them with appropriate names and values.

### Feedforward Equations

![image](https://user-images.githubusercontent.com/10822997/120015769-59431180-c001-11eb-81e2-92b5e46b8a54.png)

Write all the feedforward equations using the above diagram as reference.
Use sigmoid as the activation function for the hidden and output layers.

### Backpropagation Equation

![image](https://user-images.githubusercontent.com/10822997/120015826-6fe96880-c001-11eb-8e9a-9a44a443892f.png)

### Train a Neural Network

![image](https://user-images.githubusercontent.com/10822997/120015864-7f68b180-c001-11eb-9a70-7a0b0017b3dd.png)

Initialize all the values of the neurons and weights as shown in the neural network diagram.
Write the equations of the weights and their gradients using the above equations and choosing the right cell numbers.
Use a constant learning rate to update the weights. This will be changed to observe the effect of learning rate on loss during training.

### Loss Graphs
![image](https://user-images.githubusercontent.com/10822997/120016009-b6d75e00-c001-11eb-93e9-fbf9396f468b.png)

Observation:
We can observe that higher the value of learning rate, higher the rate of convergence of loss for this particular problem. This is not true in most deep neural network problems as the learning rate is generally kept low to update the weights slowly.
