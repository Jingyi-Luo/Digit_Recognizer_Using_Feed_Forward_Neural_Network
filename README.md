# Digit Recognizer With MNIST Data Using Feed Forward Neural Network (FFNN)

This project is aiming to recognize the gray-scale images of hand-drawn digits from zero through nine using FFNN. Moreover, the effects of number of layers, different regularization techniques (dropout, L1 regulariztion, L2 regularization), learning rates, epochs, batch sizes and width of layers have been investigated to incease the prediction accuracy of the model.

The data can be accessed here: [Data](https://www.kaggle.com/c/digit-recognizer/data)

## Architecture of FFNN

The best FFNN has four hidden layers with ReLU as the activation functions. The first, second, third and fourth hidden layers have 300, 300, 200 and 100 neurons, respectively.  The output layer outputs the logits, which then goes through the softmax activation function. We utilized cross entropy as the loss function and gradient descent optimizer to train the model. The network takes 28*28 features as the number of inputs for each instance, and outputs 10 probabilities for each class. The predicted class is determined by the highest probability among the ten.

<img width="75%" alt="tensorboard_graph" src="https://user-images.githubusercontent.com/42804316/57877884-d3bbe280-77e6-11e9-8904-69b700d92cfe.png"><img width="25%" alt="simplified_flowchart" src="https://user-images.githubusercontent.com/42804316/57877902-dd454a80-77e6-11e9-80ee-68fac531fc7e.png"><br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Fig 1. Tensorboard Computational Graph (left) and Simplified Flowchart (right)
