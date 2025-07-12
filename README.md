# ✅ Handwriting Recognition Using Convolutional Neural Networks (CNN)

## 📌 Project Overview
This project demonstrates the implementation of a **Convolutional Neural Network (CNN)** to recognize handwritten digits using the **MNIST dataset**. It involves loading and preprocessing data, building a deep learning model, evaluating accuracy, and visualizing performance metrics.

---

## 🗃️ Dataset Information
- **Dataset:** MNIST (Modified National Institute of Standards and Technology)
- **Source:** `tensorflow.keras.datasets`
- **Training Samples:** 60,000
- **Test Samples:** 10,000
- **Image Size:** 28x28 pixels
- **Number of Classes:** 10 (digits 0–9)
- **Format:** Grayscale images

---

## 📊 Data Preprocessing
- Loaded dataset using `keras.datasets.mnist.load_data()`
- Normalized pixel values by dividing by 255.0
- Visualized a sample image using `matplotlib.pyplot.imshow()`

---

## 🧠 Model Architecture

The model is built using **TensorFlow Keras** with the following architecture:

```text
Conv2D(32, (3,3), ReLU) → MaxPooling2D(2,2)  
→ Conv2D(64, (3,3), ReLU) → MaxPooling2D(2,2)  
→ Conv2D(64, (3,3), ReLU)  
→ Flatten  
→ Dense(64, ReLU)  
→ Dense(10)  (Output layer for classification)
