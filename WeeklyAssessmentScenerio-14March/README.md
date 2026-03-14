# Smart Waste Classification System

## Overview

This project builds an **AI-based image classification system** that automatically classifies waste into three categories:

* Recyclable Waste
* Organic Waste
* Non-Recyclable Waste

The system uses **Convolutional Neural Networks (CNN)** and **Transfer Learning** to improve waste segregation for smart city waste management.

---

## Dataset

Dataset source:
https://www.kaggle.com/datasets/asdasdasasdas/garbage-classification

### Dataset Structure

```
dataset/
 ├── train/
 │    ├── recyclable/
 │    ├── organic/
 │    └── non_recyclable/
 │
 └── validation/
      ├── recyclable/
      ├── organic/
      └── non_recyclable/
```

---

## Data Preprocessing

* Image resizing to **224×224**
* Pixel normalization (**rescale = 1./255**)
* Data augmentation:

  * Rotation
  * Horizontal flip
  * Zoom

---

## CNN Model

The custom CNN model includes:

* Convolution layers
* MaxPooling layers
* Dense layer
* Softmax output layer for 3-class classification

---

## Model Evaluation

Model performance evaluated using:

* **Accuracy score**
* **Confusion matrix**
* **Sample predictions on test images**

---

## Transfer Learning

A pretrained model such as **MobileNetV2 / ResNet50 / VGG16** is used to improve performance by:

* Freezing base layers
* Adding custom classification layers
* Training the model on the waste dataset

---

## Result

Transfer learning models generally achieve **higher accuracy and faster training** compared to the custom CNN model.

---

## Tools & Technologies

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn

---

## Conclusion

This project demonstrates how deep learning can be applied to **automate waste classification**, helping improve recycling and smart waste management systems.

