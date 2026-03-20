# 😊 Emotion AI – Residual CNN for Facial Emotion Recognition

## 🧠 Overview

This project implements a **facial emotion recognition system** using a **Residual Convolutional Neural Network (ResNet-inspired architecture)** trained on grayscale facial images. The model classifies human emotions and is integrated with **OpenCV** for real-time webcam-based inference.

The notebook contains the complete pipeline:
- Data preprocessing  
- Model design (Residual CNN)  
- Training & evaluation  
- Real-time deployment  

---

## 🎯 Objective

To develop a deep learning-based emotion recognition system that:
- Learns robust facial features using **residual connections**
- Achieves stable training with deeper architecture  
- Performs real-time emotion detection using webcam input  

---

## 🏗️ Methodology

### 1️⃣ Data Preprocessing

- Images are:
  - Converted to **grayscale**
  - Resized (e.g., 48×48)
  - Normalized for stable training  

- Labels are encoded for multi-class classification

---

### 2️⃣ Model Architecture – Residual CNN

The model uses **residual blocks** to improve learning in deeper networks.

#### Key Components:
- Convolutional layers  
- Residual (skip) connections  
- Batch normalization  
- ReLU activation  
- Pooling layers  
- Fully connected layers  
- Softmax output layer  

---

### 🔄 Residual Learning Concept

Instead of learning a direct mapping:
H(x)

the model learns:
F(x) + x

This helps:
- Prevent vanishing gradients  
- Improve convergence  
- Enable deeper architectures  

---

### 3️⃣ Training Setup

- **Loss Function**: Categorical Crossentropy  
- **Optimizer**: Adam  
- **Metric**: Accuracy  

---

### 4️⃣ Real-Time Inference Pipeline

Webcam → Frame Capture → Face Detection → Preprocessing → Residual CNN → Emotion Prediction

Steps:
1. Capture frame using OpenCV  
2. Detect face using Haar Cascade  
3. Extract face region  
4. Preprocess (resize + normalize)  
5. Predict emotion using trained model  
6. Display prediction on video feed  

---

## ⚙️ Implementation Details

- **Language**: Python  
- **Platform**: Google Colab / Jupyter  

### Libraries Used:
- TensorFlow / Keras  
- OpenCV  
- NumPy  

---

## 📊 Model Behavior

### ✔️ Works well for:
- Frontal faces  
- Clear expressions  
- Controlled lighting  

### ⚠️ Performance drops for:
- Low lighting  
- Occlusions  
- Non-frontal angles  

---

## 🔬 Experimental Observations

- Residual connections improve:
  - Training stability  
  - Convergence speed  
  - Feature learning  

- Grayscale input reduces computation  
- Real-time inference is feasible on CPU  

---

## 💡 Key Contributions

- Implemented a **Residual CNN for emotion classification**  
- Built an **end-to-end pipeline (training → deployment)**  
- Enabled **real-time emotion recognition using webcam**  

---

## ⚠️ Limitations

- No temporal modeling (frame-by-frame only)  
- Haar Cascade limits detection robustness  
- Performance depends on dataset diversity  

---

## 🚀 Future Work

- Replace Haar Cascade with **MTCNN / RetinaFace**  
- Use **transfer learning (ResNet50, EfficientNet)**  
- Add **temporal modeling (LSTM / Transformer)**  
- Extend to **multimodal emotion recognition (audio + video)**  

---

## 📁 Project Structure

Emotion_AI/
├── Copy_of_Emotion_AI.ipynb
├── haarcascade_frontalface_default.xml
├── emotion_model.h5

---

## ▶️ How to Run

1. Open the notebook in Google Colab or Jupyter  
2. Run all cells sequentially  
3. Upload required files:
   - Haar Cascade XML  
   - Model file (if loading pretrained)  
4. Enable webcam access  
5. Observe real-time predictions  

---

## 📦 Requirements

pip install tensorflow keras opencv-python numpy

---

## 😊 Emotion Classes

- Happy  
- Sad  
- Angry  
- Surprise  
- Neutral  

---

## ✍️ Author

**Sai Sohan Sajja**  
Machine Learning | Computer Vision | Affective AI  | Natural Language Processing

---


- Validation Accuracy: XX%  
