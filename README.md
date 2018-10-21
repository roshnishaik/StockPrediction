# A simple deep learning model for stock prediction using TensorFlow

This repository contains the Python script as well as the source dataset. The dataset contains n = 41266 minutes of data ranging from April to August 2017 on 500 stocks as well as the total S&P 500 index price. Index and stocks are arranged in wide format. The dataset was split into training and test data. The training data contained 80% of the total dataset.

The model consists of four hidden layers. The first layer contains 1024 neurons. Subsequent hidden layers are always half the size of the previous layer, which means 512, 256 and finally 128 neurons. A reduction of the number of neurons for each subsequent layer compresses the information the network identifies in the previous layers.

The hidden layers of the network are transformed by activation functions. Activation functions are important elements of the network architecture since they introduce non-linearity to the system. There are dozens of possible activation functions out there, one of the most common is the rectified linear unit (ReLU) which will also be used in this model.

The model consists of three major building blocks. The input layer, the hidden layers and the output layer. This architecture is called a feedforward network. Feedforward indicates that the batch of data solely flows from left to right. Other network architectures, such as recurrent neural networks, also allow data flowing “backwards” in the network.
 
Mean squared error function is used as cost function. It computes the average squared deviation between predictions and targets.

Adaptive Moment Estimation optimizer is used to take care of necessary computations that are used to adapt network’s weight and bias variables during training.
