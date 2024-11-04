java c159.740 Intelligent Systems
Assignment #2 
N.H.Reyes 
Letter Recognition using Deep Neural Nets with Softmax Units 
Deadline: 4th of November 
Instructions: 
You are allowed to work in a group of 2 members for this assignment. 
Your task is to write a program that implements and tests a multi-layer feed-forward network for 
recognising characters defined in the UCI machine learning repository: 
http://archive.ics.uci.edu/ml/datasets/Letter+Recognition
Requirements: 
1. Use QT to develop your Neural Network application. A short tutorial on QT, and a start-up 
code that will help you get started quickly with the assignment is provided via Stream. 
2. You may utilise/consult codes available in books and websites provided that you cite them 
properly, explain the codes clearly, and incorporate them with the start-up codes provided. 
3. Implement a multi-layer feed-forward network using backpropagation learning and test it on the 
given problem domain using different network configurations and parameter settings. There 
should be at least 2 hidden layers in your neural network. 
h21 h11 X1
X2
F1
F2 h12 h22
OF1
OF2
δh21
δh22 δh12
δf1
δf2
δh11
… … … … 
X16
Fm Hi Hj
OFm
Input node
Legend: 
hidden node
output node = softmax unit
 Note that all nodes, except the input nodes have a bias node attached to it. 
159.740 Intelligent Systems
Assignment #2 
N.H.Reyes 
A. Inputs 
 16 primitive numerical attributes (statistical moments and edge counts) 
 The input values in the data set have been scaled to fit into a range of integer values 
from 0 through 15. It is up to you if you want to normalise the inputs before feeding 
them to your network. 
B. Data sets 
 Use the data set downloadable from: 
 Training set: use the first 16,000 
 Test set/Validation set: use the remaining 4,000 
 Submit your training data, validation/test data in separate files. 
C. Performance measure: 
 Mean Squared Error (MSE) 
 Percentage of Good Classification (PGC) 
 Confusion Matrix (only for the best Neural Network configuration found) 
D. Training 
 Provide a facility for shuffling data before feeding it to the network during training 
 Provide a facility for continuing network training after loading weights from file (do not 
reset the weights). 
 Provide a facility for training the network continuously until either the maximum 
epochs have been reached, or the target percentage of good classification has been met. 
 For each training epoch, record the Mean Squared Error and the Percentage of Good 
Classification in a text file. You need this to plot the results of training later, to 
compare the effects of the parameter settings and the architecture of your network. 
E. Testing the Network 
 Calculate the performance of the network on the Test set in terms of both the MSE and 
PGC. 
F. Network Architecture 
 It is up to yo代 写159.740、c/c++，Python
代做程序编程语言u to determine the number of hidden layers and number of hidden nodes 
per hidden layer in your network. The minimum number of hidden layers is 2. 
 Use softmax units at the output layer 
 Experiment with ReLU and tanh as the activation functions of your hidden units 
 Determine the weight-update formulas based on the activation functions used 
4. Provide an interface in your program for testing the network using an input string consisting of 
the 16 attributes. The results should indicate the character classification, and the 26 actual 
numeric outputs of the network. (the start-up codes partly include this functionality already, for 
a simple 3-layer network (1 hidden layer), but you need to modify it to make it work for the 
multiple hidden layer architecture that you have designed). 
5. Provide an interface in your program for: 
A. Reading the entire data set 
B. Initialising the network 
C. Loading trained weights 
D. Saving trained weights 
E. Training the network up to a maximum number of epochs 
159.740 Intelligent Systems
Assignment #2 
F. Testing the network on a specified test set (from a file) 
G. Shuffling the training set. 
6. Set the default settings of the user interface (e.g. learning rate, weights, etc.) to the best 
configuration that delivered the best experiment results. 
7. Use a fixed random seed number (123) so that any randomisation can be replicated empirically. 
8. It is up to you to write the main program, and any classes or data structures that you may 
require. 
9. You may choose to use a momentum term or regularization term, as part of backpropagation 
learning. Indicate in your documentation, if you are using this technique. 
10. You need to modify the weight-update rules to reflect the correct derivatives of the activation 
function used in your network architecture. 
11. Provide graphs in Excel showing the network performance on training data and test data 
(similar to the graphs discussed in the lecture). 
12. Provide the specifications of your best trained network. Fill-up Excel workbook 
(best_network_configuration.xlsx). 
13. Provide a confusion matrix for the best NN classifier system found in your experiments. 
14. Provide a short user guide for your program. 
15. Fill-up the Excel file, named checklist.xlsx, to allow for accurate marking of your assignment. 
Criteria for marking 
 Documentation – 30% 
o Submit the trained weights of your best network (name it as best_weights.txt) 
o Generate a graph of the performance of your best performing network (MSE vs. 
Epochs) on the training set and test set. 
o Generate a confusion matrix of your best network 
o fill-up the Excel file, named checklist.xlsx
o fill-up the Excel file, named best_network_configuration.xlsx
o provide a short user guide for your program 
 System implementation – 70% 
Nothing follows. 
N.H.Reyes 

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
