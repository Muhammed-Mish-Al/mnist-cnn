# mnist-cnn
# InternSpot MNIST Digit Recognition

A handwritten digit recognition project built with a LeNet-5 Convolutional Neural Network (CNN) and the MNIST dataset as part of my InternSpot learning journey.

## Project Overview

This model learns to identify handwritten digits from 0 to 9. It is trained on MNIST, a dataset containing 60,000 training images and 10,000 test images.

The project uses the LeNet-5 CNN architecture to extract visual features from grayscale digit images and classify them into one of ten digit classes.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

## Model Architecture

The model follows the LeNet-5 architecture:

1. Conv2D — 6 filters, 5 × 5 kernel, tanh activation
2. Average Pooling
3. Conv2D — 16 filters, 5 × 5 kernel, tanh activation
4. Average Pooling
5. Conv2D — 120 filters, 5 × 5 kernel, tanh activation
6. Flatten
7. Dense — 84 neurons, tanh activation
8. Output Dense — 10 neurons, softmax activation

## Dataset

MNIST contains grayscale images of handwritten digits.

- Training images: 60,000
- Test images: 10,000
- Image size: 28 × 28 pixels
- Classes: 10 digits, from 0 to 9

## Results

The model achieved approximately **98% test accuracy** on unseen MNIST images.

## How to Run

1. Clone this repository.

```bash
git clone https://github.com/YOUR-USERNAME/internspot-mnist-digit-recognition.git
```

2. Install the required libraries.

```bash
pip install tensorflow numpy pandas scikit-learn jupyter
```

3. Open Jupyter Notebook.

```bash
jupyter notebook
```

4. Open the project notebook and run every cell from top to bottom.

## What I Learned

- Loading and preparing image datasets
- Reshaping grayscale images for CNN input
- Standardizing pixel values
- One-hot encoding labels
- Building a LeNet-5 CNN with TensorFlow and Keras
- Training, validating, and evaluating a deep-learning model

## Author

Built by **YOUR NAME** as an InternSpot project.
