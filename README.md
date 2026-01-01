# CNN Based Face Mask Detection Project

This project demonstrates the implementation of a **Convolutional Neural Network (CNN)** for **image classification**, with a practical use case in **Face Mask Detection**.  
It follows a complete deep learning pipeline including data preprocessing, CNN architecture design, training, evaluation, and prediction.

---

## 📌 Project Overview

The objective of this project is to build a CNN model capable of classifying images into predefined categories such as **Mask** and **No Mask**.  
The project helps in understanding how CNNs automatically extract features from images and make accurate predictions.

---

## 📁 Project Contents

- Image datasets (training and testing)
- CNN model implementation
- Model training and evaluation
- Prediction on new images or video frames
- Face Mask Detection use case

---

## 🧠 Why CNN for This Project?

- CNNs are specifically designed for image data
- They automatically extract spatial features like edges, shapes, and textures
- They outperform traditional neural networks in computer vision tasks

---

## 🔹 Dataset Loading & Preparation

### What happens:
- Images are loaded from directory structure
- Each folder represents a class (e.g., Mask / No Mask)
- Images are resized to a fixed shape

### Why needed:
- CNN requires uniform image dimensions
- Directory-based labeling simplifies supervised learning

---

## 🔹 Image Preprocessing

### Key operations:
- Rescaling pixel values (0–255 → 0–1)
- Data augmentation (rotation, zooming, flipping)
- Batch-wise image loading

### Purpose:
- Improves model generalization
- Reduces overfitting
- Makes the model robust to real-world variations

---

## 🔹 Convolution Layer (CNN ReLU Layer)

### Function:
- Applies filters (kernels) to input images
- Extracts low-level and high-level features

### Activation:
- ReLU (Rectified Linear Unit)

### Why ReLU:
- Adds non-linearity
- Faster training
- Prevents vanishing gradient problem

---

## 🔹 Max Pooling Layer

### Function:
- Downsamples feature maps
- Retains the most important features

### Benefits:
- Reduces computation
- Prevents overfitting
- Makes the model invariant to small position changes

---

## 🔹 Flattening Layer

### Function:
- Converts 2D feature maps into a 1D vector

### Why required:
- Fully connected layers accept only 1D input
- Acts as a bridge between CNN and ANN layers

---

## 🔹 Fully Connected (Dense) Layer

### Function:
- Performs high-level reasoning
- Combines extracted features for classification

### Role:
- Learns complex patterns from extracted image features

---

## 🔹 Output Layer

### Function:
- Produces final prediction

### Activation Used:
- **Sigmoid** → Binary classification (Mask / No Mask)
- **Softmax** → Multi-class classification

---

## 🔹 Model Compilation

### Components:
- Optimizer: Adam
- Loss Function: Binary Crossentropy / Categorical Crossentropy
- Metric: Accuracy

### Why Adam:
- Adaptive learning rate
- Faster convergence

---

## 🔹 Model Training

### What happens:
- Model learns patterns from training images
- Weights updated using backpropagation
- Training performed over multiple epochs

### Key Terms:
- Epoch
- Batch size
- Validation data

---

## 🔹 Model Evaluation

### Purpose:
- Measure accuracy on unseen data
- Check overfitting or underfitting

### Outcome:
- Ensures model generalization

---

## 🔹 Prediction on New Images / Video

### Process:
- Input image or video frame is captured
- Same preprocessing is applied
- CNN predicts class label

### Use Case:
- Real-time face mask detection
- Image classification applications

---

## 🧑‍🦱 How CNN is Used in Face Mask Detection

### Step-by-step usage:
1. Face is detected from an image or video frame
2. The face region is extracted and resized
3. CNN processes the face image
4. Features like nose, mouth, and facial shape are analyzed
5. Model predicts:
   - **Mask**
   - **No Mask**

### Why CNN is effective:
- Learns facial patterns automatically
- Works well with real-world images
- High accuracy in visual recognition tasks

---

## 🔄 CNN vs ANN

| CNN | ANN |
|---|---|
| Designed for images | Designed for tabular data |
| Automatic feature extraction | Manual feature engineering |
| Uses convolution & pooling | Uses fully connected layers |

---

## 🎯 Learning Outcomes

- Strong understanding of CNN architecture
- Hands-on experience with image preprocessing
- Practical exposure to computer vision
- Real-world application in face mask detection

---

## ⏱️ 30-Second Project Explanation

> I built a CNN-based image classification model for face mask detection. The project includes image preprocessing, convolution and pooling layers for feature extraction, and dense layers for classification. The model predicts whether a person is wearing a mask using sigmoid activation, making it suitable for real-time face detection systems.

---

## 👤 Author

**Yatnesh Sokal**
