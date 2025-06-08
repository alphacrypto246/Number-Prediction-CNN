# Number Prediction with TensorFlow

This repository contains a Jupyter Notebook (`Number_Prediction.ipynb`) that demonstrates a simple neural network model for digit classification using the MNIST dataset and TensorFlow.

## Overview

The notebook trains a neural network to classify handwritten digits (0-9) from the MNIST dataset. It uses a single-layer dense neural network with TensorFlow and Keras to achieve this task.

## Requirements

To run the notebook, you need the following dependencies:
- Python 3.x
- TensorFlow
- NumPy
- Matplotlib

You can install the required packages using:
```bash
pip install tensorflow numpy matplotlib
```

## Notebook Structure

1. **Install TensorFlow**: Installs the TensorFlow library.
2. **Import Libraries**: Imports necessary libraries including TensorFlow, Keras, NumPy, and Matplotlib.
3. **Load MNIST Dataset**: Loads the MNIST dataset, which consists of 60,000 training images and 10,000 test images of handwritten digits.
4. **Data Exploration**: Checks the size and shape of the dataset and visualizes a sample image.
5. **Data Preprocessing**: Normalizes pixel values to the range [0, 1] and flattens the 28x28 images into 1D arrays of 784 elements.
6. **Model Definition**: Defines a simple sequential model with one dense layer using a sigmoid activation function.
7. **Model Compilation and Training**: Compiles the model with the Adam optimizer and sparse categorical crossentropy loss, then trains it for 10 epochs.

## How to Run

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the repository directory:
   ```bash
   cd <repository-directory>
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Number_Prediction.ipynb
   ```
4. Run all cells in the notebook to train the model and view results.

## Results

The model achieves decent accuracy on the MNIST dataset after 10 epochs, as shown in the training output. You can evaluate the model's performance on the test set by adding evaluation code (e.g., `model.evaluate(X_test_flatten, y_test)`).

## License

This project is licensed under the MIT License.

## Acknowledgments

- [TensorFlow Documentation](https://www.tensorflow.org/)
- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)
