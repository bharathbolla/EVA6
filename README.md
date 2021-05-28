
# Part-1

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

# Part-2
On MNIST data, create a model to get 
99.4% validation accuracy
Less than 20k Parameters
You can use anything from above you want. 
Less than 20 Epochs
Have used BN, Dropout, a Fully connected layer, have used GAP. 

### Final Results
1. Achieved 99.4 test accuracy in 15th epoch
2. Total Parameters 9848
3. Droput = 0.04
4. Augmentation = Yes
5. Optimizer = SGD 
6. BatchNorm  = Yes
7. 1x1 Con Layer = Yes, 2 times
8. Max Channels = 20

### Model Architecture
![image](https://user-images.githubusercontent.com/10822997/120017277-52b59980-c003-11eb-828f-e002e84af90d.png)

2 3x3 conv layers followed by 1 1x1 con layer
![image](https://user-images.githubusercontent.com/10822997/120017445-8395ce80-c003-11eb-8d08-9335c3956bee.png)
![image](https://user-images.githubusercontent.com/10822997/120017555-a3c58d80-c003-11eb-972c-bfb5a821c568.png)

### Model Results
  0%|          | 0/1875 [00:00<?, ?it/s]epoches: 1
/usr/local/lib/python3.7/dist-packages/ipykernel_launcher.py:84: UserWarning: Implicit dimension choice for log_softmax has been deprecated. Change the call to include dim=X as an argument.
Loss=0.1682090163230896 Batch_id=1874 Accuracy=91.70: 100%|██████████| 1875/1875 [00:25<00:00, 73.02it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0532, Accuracy: 9834/10000 (98.34%)

epoches: 2
Loss=0.04723441228270531 Batch_id=1874 Accuracy=97.19: 100%|██████████| 1875/1875 [00:25<00:00, 72.21it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0388, Accuracy: 9874/10000 (98.74%)

epoches: 3
Loss=0.03079293854534626 Batch_id=1874 Accuracy=97.60: 100%|██████████| 1875/1875 [00:25<00:00, 73.86it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0321, Accuracy: 9895/10000 (98.95%)

epoches: 4
Loss=0.003184626577422023 Batch_id=1874 Accuracy=97.89: 100%|██████████| 1875/1875 [00:25<00:00, 72.77it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0261, Accuracy: 9910/10000 (99.10%)

epoches: 5
Loss=0.024312244728207588 Batch_id=1874 Accuracy=98.11: 100%|██████████| 1875/1875 [00:26<00:00, 71.98it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0258, Accuracy: 9912/10000 (99.12%)

epoches: 6
Loss=0.0924961194396019 Batch_id=1874 Accuracy=98.25: 100%|██████████| 1875/1875 [00:25<00:00, 72.61it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0207, Accuracy: 9931/10000 (99.31%)

epoches: 7
Loss=0.05757199600338936 Batch_id=1874 Accuracy=98.31: 100%|██████████| 1875/1875 [00:26<00:00, 72.03it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0226, Accuracy: 9920/10000 (99.20%)

epoches: 8
Loss=0.24231401085853577 Batch_id=1874 Accuracy=98.37: 100%|██████████| 1875/1875 [00:25<00:00, 73.19it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0204, Accuracy: 9926/10000 (99.26%)

epoches: 9
Loss=0.00595014076679945 Batch_id=1874 Accuracy=98.44: 100%|██████████| 1875/1875 [00:26<00:00, 71.35it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0219, Accuracy: 9931/10000 (99.31%)

epoches: 10
Loss=0.005863219499588013 Batch_id=1874 Accuracy=98.48: 100%|██████████| 1875/1875 [00:25<00:00, 73.14it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0232, Accuracy: 9913/10000 (99.13%)

epoches: 11
Loss=0.0951457992196083 Batch_id=1874 Accuracy=98.59: 100%|██████████| 1875/1875 [00:26<00:00, 72.10it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0233, Accuracy: 9929/10000 (99.29%)

epoches: 12
Loss=0.0397578626871109 Batch_id=1874 Accuracy=98.59: 100%|██████████| 1875/1875 [00:26<00:00, 71.80it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0184, Accuracy: 9938/10000 (99.38%)

epoches: 13
Loss=0.010606668889522552 Batch_id=1874 Accuracy=98.69: 100%|██████████| 1875/1875 [00:25<00:00, 72.79it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0233, Accuracy: 9927/10000 (99.27%)

epoches: 14
Loss=0.02882736176252365 Batch_id=1874 Accuracy=98.66: 100%|██████████| 1875/1875 [00:26<00:00, 71.54it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0221, Accuracy: 9925/10000 (99.25%)

epoches: 15
Loss=0.01114226970821619 Batch_id=1874 Accuracy=98.72: 100%|██████████| 1875/1875 [00:26<00:00, 71.01it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0171, Accuracy: 9944/10000 (99.44%)

epoches: 16
Loss=0.017643120139837265 Batch_id=1874 Accuracy=98.64: 100%|██████████| 1875/1875 [00:26<00:00, 71.01it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0187, Accuracy: 9941/10000 (99.41%)

epoches: 17
Loss=0.002063074382022023 Batch_id=1874 Accuracy=98.72: 100%|██████████| 1875/1875 [00:25<00:00, 72.37it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0188, Accuracy: 9935/10000 (99.35%)

epoches: 18
Loss=0.012451915070414543 Batch_id=1874 Accuracy=98.75: 100%|██████████| 1875/1875 [00:26<00:00, 71.65it/s]
  0%|          | 0/1875 [00:00<?, ?it/s]
Test set: Average loss: 0.0196, Accuracy: 9938/10000 (99.38%)

epoches: 19
Loss=0.006165508180856705 Batch_id=1874 Accuracy=98.80: 100%|██████████| 1875/1875 [00:26<00:00, 70.91it/s]

Test set: Average loss: 0.0213, Accuracy: 9930/10000 (99.30%)
