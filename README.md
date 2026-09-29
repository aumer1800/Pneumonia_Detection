# Pneumonia Detection using CNN

A deep learning project that uses a **Convolutional Neural Network (CNN)** to classify chest X-ray images into two classes:

* NORMAL
* PNEUMONIA

## Project Overview

The model takes a chest X-ray image as input and predicts whether it is **Normal** or shows **Pneumonia**.

The project was developed using **Python and TensorFlow/Keras** and can be trained using Google Colab.

## Dataset

**Chest X-Ray Pneumonia Dataset**

The dataset contains chest X-ray images divided into:

* Training data
* Validation data
* Test data

The images are resized to **150 × 150 pixels** before being given to the model.

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Scikit-learn
* Seaborn
* Google Colab

## Data Preprocessing

The following preprocessing techniques are used:

* Resize images to 150 × 150
* Normalize pixel values between 0 and 1
* Rotate images randomly
* Apply zoom augmentation
* Apply horizontal flipping
* Split training data into training and validation sets
* Handle class imbalance using class weights

## CNN Architecture

The model consists of:

1. Input Layer
2. Convolutional Layer
3. ReLU Activation
4. Max Pooling
5. Convolutional Layer
6. Max Pooling
7. Convolutional Layer
8. Max Pooling
9. Convolutional Layer
10. Max Pooling
11. Flatten Layer
12. Dropout Layer
13. Dense Layer
14. Sigmoid Output Layer

The output layer produces a probability for the **PNEUMONIA** class.

## Model Training

The model uses:

* **Optimizer:** Adam
* **Learning Rate:** 0.0001
* **Loss:** Binary Crossentropy
* **Metric:** Accuracy
* **Maximum Epochs:** 50
* **Early Stopping:** Enabled

Class weights are also used to help handle class imbalance.

## Model Evaluation

The trained model is evaluated using unseen test images.

The project includes:

* Test Accuracy
* Test Loss
* Training and Validation Accuracy
* Training and Validation Loss
* Confusion Matrix
* Classification Report
* Precision
* Recall
* F1-Score

## Model Output

The trained model is saved in Keras format:

```text
pneumonia_cnn_model.keras
```

## Project Workflow

```text
Chest X-Ray Images
        ↓
Data Preprocessing
        ↓
Data Augmentation
        ↓
CNN Model
        ↓
Model Training
        ↓
Model Evaluation
        ↓
NORMAL / PNEUMONIA
```

## Future Improvements

* Use transfer learning models
* Improve model accuracy
* Add more evaluation metrics
* Deploy the model as a web application
* Add an image upload interface for predictions

## Disclaimer

This project is intended for **educational and research purposes**. It is not a replacement for professional medical diagnosis.
