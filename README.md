# MNIST Handwritten Digit Recognition Using CNN

## Overview
This project uses a Convolutional Neural Network (CNN) to recognize handwritten digits from 0 to 9 using the MNIST dataset.

## Dataset
- **Dataset:** MNIST
- **Total images:** 70,000
- **Image size:** 28 × 28 pixels
- **Image type:** Grayscale
- **Classes:** Digits 0–9

## Technologies
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Key Features
- Handwritten digit image preprocessing
- CNN model development and training
- Ten-class digit classification
- Model evaluation using test data
- Visualization of predictions and training performance

## Project Workflow
1. Load the MNIST dataset.
2. Normalize the images and prepare the labels.
3. Build and train the CNN model.
4. Evaluate the model on test data.
5. Visualize predictions and performance.

## Installation
Install the required libraries:

```bash
pip install tensorflow numpy matplotlib scikit-learn jupyter
```

## How to Run
1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `MNIST_CNN_Digit_Recognition.ipynb`.
5. Run the notebook cells in order.

## Evaluation
The model's performance can be assessed using test accuracy, loss curves, and a confusion matrix, where implemented in the notebook.

## Future Improvements
- Test different CNN architectures.
- Tune hyperparameters for improved performance.
- Analyze incorrectly classified digits.
- Develop an interface for predicting digits from user-provided images.
