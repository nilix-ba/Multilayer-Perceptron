# Multilayer Perceptron (MLP) Readme

## Overview

This repository contains the code for a Multilayer Perceptron (MLP) implemented in Python. The MLP is a type of artificial neural network that can be used for classification tasks. The code includes the implementation of the MLP, training, and testing it on a dataset.

## Code Structure

The code is organized into several sections, each serving a specific purpose:

1. **Importing Libraries**:
    - The code starts by importing necessary libraries, including NumPy, Math, Matplotlib, and OS.

2. **Matrix Multiplication Function**:
    - The `matmul` function is defined to perform matrix multiplication between two matrices.

3. **Neural Network Class**:
    - The `NeuralNetwork` class is defined to represent the MLP.
    - The constructor `__init__` initializes the neural network with the number of input, hidden, and output nodes. It also initializes weights and biases with random values.
    - The `sigmoid` and `sigmoidp` methods define the sigmoid activation function and its derivative.
    - The `feedforward` method performs a forward pass through the network to generate predictions.
    - The `train` method performs backpropagation and updates the weights and biases during training.

4. **Input Data Reader**:
    - The `reader` function reads input data from a file and returns it as a list of lists.

5. **Main Part**:
    - In the main part of the code, an instance of the `NeuralNetwork` class is created with specific input, hidden, and output node counts.
    - Training and testing data are read from files ("train" and "test").
    - The neural network is trained for 4000 iterations using the training data.
    - The trained network is then tested on the testing data, and the accuracy of the predictions is calculated.
    - The code also generates scatter plots of the testing data points, colored by their predicted class.

## Usage

To use this code, follow these steps:

1. Ensure you have Python installed on your system.

2. Clone or download this repository to your local machine.

3. Create training and testing data files. Each file should contain one data point per line, with features separated by spaces, followed by the class label (0 or 1).

4. Modify the main part of the code to specify the correct file paths and adjust the network architecture if needed.

5. Run the code using a Python interpreter.

## Dependencies

This code depends on the following Python libraries:
- NumPy
- Matplotlib

You can install these libraries using pip if they are not already installed:

```bash
pip install numpy matplotlib
```

