# Fashion-MNIST Image Classification using Multi-Layer Perceptron (MLP)

## Project Overview

This project implements a **Multi-Layer Perceptron (MLP)** using **TensorFlow/Keras** to classify images from the **Fashion-MNIST dataset** into one of ten clothing categories.

The project covers data preprocessing, exploratory data analysis (EDA), neural network training, performance evaluation, hyperparameter tuning using **RandomizedSearchCV**, and visualization of training performance.

---

## Dataset

**Dataset:** Fashion-MNIST

**Source:** TensorFlow/Keras Datasets

The Fashion-MNIST dataset consists of grayscale images of clothing items.

### Dataset Information

- Training Images: **60,000**
- Testing Images: **10,000**
- Image Size: **28 × 28 pixels**
- Number of Classes: **10**

### Classes

| Label | Class |
|------|----------------|
| 0 | T-shirt/Top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

## Project Workflow

1. Load the Fashion-MNIST dataset
2. Explore the dataset
3. Visualize sample images and class distribution
4. Preprocess the data
5. Build a Multi-Layer Perceptron (MLP)
6. Train the neural network
7. Evaluate model performance
8. Perform hyperparameter tuning using RandomizedSearchCV
9. Compare baseline and optimized models

---

## Exploratory Data Analysis (EDA)

The project includes the following visualizations:

- Sample Fashion-MNIST Images
- Class Distribution

These visualizations help understand the dataset and verify class balance.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Flattened 28 × 28 images into 784-dimensional vectors
- Normalized pixel values to the range **0–1**
- One-hot encoded class labels using `to_categorical()`

---

## Model Architecture

The baseline neural network consists of:

- Input Layer (784 neurons)
- Hidden Layer 1 (128 neurons, ReLU)
- Hidden Layer 2 (64 neurons, ReLU)
- Output Layer (10 neurons, Softmax)

### Loss Function

- Categorical Crossentropy

### Optimizer

- Adam

### Evaluation Metric

- Accuracy

---

## Hyperparameter Tuning

Randomized Search Cross Validation was performed using **Scikeras** and **RandomizedSearchCV**.

The following hyperparameters were tuned:

- Number of Hidden Layers
- Number of Neurons
- Learning Rate
- Activation Function
- Optimizer
- Dropout Rate
- Batch Size
- Number of Epochs

---

## Model Evaluation

The trained model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

---

## Visualizations

The project includes the following plots:

- Training Accuracy vs Epoch
- Validation Accuracy vs Epoch
- Training Loss vs Epoch
- Validation Loss vs Epoch
- Random Search Cross Validation Accuracy
- Baseline vs Optimized Model Accuracy
- Confusion Matrix
- Sample Fashion-MNIST Images
- Class Distribution

---

## Libraries Used

- NumPy
- Pandas
- Matplotlib
- Seaborn
- TensorFlow
- Keras
- Scikit-learn
- Scikeras

---

## Project Structure

```
Fashion-MNIST-MLP/
│
├── MLP.ipynb
├── MLP.py
├── README.md
├── requirements.txt
└── images/ (optional)
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/your-username/Fashion-MNIST-MLP.git
```

Move into the project directory

```bash
cd Fashion-MNIST-MLP
```

Install the required libraries

```bash
pip install -r requirements.txt
```

Run the Python script

```bash
python MLP.py
```

or open

```
MLP.ipynb
```

using Jupyter Notebook or Google Colab.

---

## Results

The Multi-Layer Perceptron successfully classifies Fashion-MNIST images with high accuracy. Training and validation curves demonstrate effective learning, while hyperparameter tuning further improves the model's performance. The confusion matrix and classification report provide detailed insights into classification accuracy across all clothing categories.

---

## Future Improvements

- Convolutional Neural Networks (CNN)
- Batch Normalization
- Early Stopping
- Learning Rate Scheduling
- Data Augmentation
- Transfer Learning using Pre-trained Models

---
