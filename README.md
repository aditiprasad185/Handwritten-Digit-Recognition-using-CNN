MNIST Handwritten Digit Recognition using Convolutional Neural Networks (CNN)

📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** using TensorFlow and Keras to recognize handwritten digits from the MNIST dataset.

The model classifies grayscale images into one of 10 digit classes, ranging from 0 to 9. The project demonstrates image preprocessing, CNN model development, model training, evaluation, prediction visualization, and saving the trained model.

🎯 Objectives

- Build a CNN model for handwritten digit recognition.
- Load and preprocess the MNIST dataset.
- Normalize pixel values and reshape images for CNN input.
- Train the model using TensorFlow and Keras.
- Evaluate model performance on unseen test images.
- Visualize model accuracy, loss, and confusion matrix.
- Predict individual handwritten digits.
- Save the trained model for future use.

📂 Dataset

The project uses the **MNIST handwritten digit dataset**, a standard dataset for image classification.

- Total images: 70,000
- Training images: 60,000
- Testing images: 10,000
- Image dimensions: 28 × 28 pixels
- Image channels: 1 (grayscale)
- Number of classes: 10 (digits 0–9)

The dataset is loaded directly using `keras.datasets.mnist.load_data()`.

Target Classes

The model predicts one of the following digit classes:

`0, 1, 2, 3, 4, 5, 6, 7, 8, 9`

🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

🧠 Model Architecture

The CNN model is built using the Keras Sequential API.

The architecture consists of:

1. Input Layer: Accepts grayscale images of size 28 × 28 × 1.
2. Convolutional Layer: 32 filters with a 3 × 3 kernel and ReLU activation.
3. Max Pooling Layer: Reduces the spatial dimensions of feature maps.
4. Convolutional Layer: 64 filters with a 3 × 3 kernel and ReLU activation.
5. Max Pooling Layer: Further reduces spatial dimensions.
6. Flatten Layer: Converts feature maps into a one-dimensional vector.
7. Dense Layer: 64 neurons with ReLU activation.
8. Dropout Layer: Dropout rate of 0.3 to help reduce overfitting.
9. Output Layer: 10 neurons with Softmax activation to predict digit probabilities.

Training Configuration

- Optimizer: Adam
- Loss function: Sparse categorical cross-entropy
- Evaluation metric: Accuracy
- Maximum epochs: 15
- Batch size: 128
- Validation split: 20%
- Early stopping patience: 3 epochs
- Model checkpoint: Saves the best model based on validation loss

⚙️ Installation and Setup

1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

2. Install the required libraries

```bash
pip install tensorflow numpy matplotlib scikit-learn jupyter
```

3. Launch Jupyter Notebook

```bash
jupyter notebook
```

4. Run the notebook

Open `MNIST_CNN_Digit_Recognition.ipynb` and execute the cells sequentially.

The MNIST dataset will be downloaded automatically when it is first loaded, if it is not already available locally.

🚀 Project Workflow

1. Import the required libraries.
2. Load the MNIST training and testing datasets.
3. Visualize sample handwritten digits.
4. Normalize pixel values to the range 0–1.
5. Add a channel dimension to the grayscale images.
6. Build the CNN model.
7. Compile the model using Adam and sparse categorical cross-entropy.
8. Train the model with validation data.
9. Apply early stopping and model checkpointing.
10. Plot training and validation accuracy and loss.
11. Evaluate the model on the test dataset.
12. Generate a confusion matrix.
13. Predict a digit from an individual test image.
14. Display the predicted digit and its probability distribution.
15. Save the trained model.

📊 Model Evaluation

The model is evaluated using the following methods:

- **Test Accuracy:** Measures the percentage of correctly recognized digits.
- **Test Loss:** Measures prediction error on the test dataset.
- **Confusion Matrix:** Shows correct and incorrect classifications for each digit.
- **Training and Validation Curves:** Visualize the model's learning progress.
- **Individual Digit Prediction:** Compares the actual digit with the predicted digit
