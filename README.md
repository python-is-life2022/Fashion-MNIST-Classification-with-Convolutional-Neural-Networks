# Fashion-MNIST Image Classification using CNN

A Deep Learning project for classifying Fashion-MNIST images using a Convolutional Neural Network (CNN) built with TensorFlow and Keras.

## 📌 Project Overview

In this project, I built and evaluated a Convolutional Neural Network (CNN) to classify images from the Fashion-MNIST dataset.

The main goal was not only to build a CNN model, but also to understand how different hyperparameters and architectural choices affect model performance and overfitting.

Throughout the project, I experimented with different Learning Rates, Dropout configurations, and numbers of Epochs to find a suitable configuration for the model.

---

## 📊 Dataset

The project uses the **Fashion-MNIST** dataset provided by Keras.

The dataset contains:

- **60,000** training images
- **10,000** test images
- **10 different classes**
- Image size: **28 × 28 pixels**
- Grayscale images

The 10 classes represent different types of clothing and fashion items.

### Classes

1. T-shirt / Top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle Boot

---

## 🔀 Data Splitting

Instead of using all training data directly for model fitting, **25% of the training data was separated as validation data**.

This validation set was used during training to monitor the model's performance on unseen data and to help identify potential overfitting.

The original test set remained completely separate and was used for the final evaluation of the model.

---

## 🧠 CNN Architecture

The model was designed using multiple convolutional blocks.

The number of filters increases progressively:

```text
32 → 64 → 128
