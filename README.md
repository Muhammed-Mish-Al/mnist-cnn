# mnist-cnn
# MNIST Digit Recognition

A deep-learning project that classifies handwritten digits (0–9) using a LeNet-5 Convolutional Neural Network (CNN) trained on the MNIST dataset.

## Overview

This project builds and evaluates a CNN for handwritten digit recognition. The model processes grayscale images, extracts visual features through convolution and pooling layers, and predicts the corresponding digit class.

## Dataset

The MNIST dataset contains handwritten digit images:

- 60,000 training images
- 10,000 test images
- Image dimensions: 28 × 28 pixels
- Classes: digits 0 through 9

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

## Model Architecture

The model is based on LeNet-5 and includes:

1. Conv2D — 6 filters, 5 × 5 kernel, tanh activation
2. Average Pooling
3. Conv2D — 16 filters, 5 × 5 kernel, tanh activation
4. Average Pooling
5. Conv2D — 120 filters, 5 × 5 kernel, tanh activation
6. Flatten
7. Dense — 84 neurons, tanh activation
8. Output layer — 10 neurons, softmax activation

## Workflow

- Load the MNIST dataset
- Reshape images to include a grayscale channel
- Split training data into training and validation sets
- Standardize pixel values
- One-hot encode digit labels
- Train the LeNet-5 CNN
- Evaluate the final model on unseen test images

## Results

The reference implementation achieved approximately **98.24% test accuracy**. Results may vary slightly between runs.

## How to Run

1. Clone the repository.

```bash
git clone https://github.com/Muhammed-Mish-Al/internspot-mnist.git
```

2. Open the project folder.

```bash
cd internspot-mnist
```

3. Install the required libraries.

```bash
pip install tensorflow numpy pandas scikit-learn jupyter
```

4. Start Jupyter Notebook.

```bash
jupyter notebook
```

5. Open `mnist_digit_recognition.ipynb` and run all cells from top to bottom.

## Author

**Muhammed Mish_Al**

Completed as part of the **InternSpot Internship**.
