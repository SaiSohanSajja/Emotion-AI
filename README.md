# 😊 Emotion Detection AI – Real-time Facial Emotion Recognition

This project uses computer vision and deep learning to detect **human emotions from facial expressions** in real time. It combines **OpenCV** for face detection and **a trained deep learning model** (CNN) to classify facial emotions such as happy, sad, angry, surprised, and neutral.

---

## 🔍 Project Overview

- **Goal**: Identify and classify facial emotions in real time using webcam input.
- **Approach**: Face detection with OpenCV, emotion classification with CNN.
- **Output**: Live video feed with emotion labels overlaid on detected faces.

---

## 🛠️ Features

- ✅ Real-time webcam capture  
- ✅ Face detection using Haar cascades  
- ✅ Emotion classification (happy, sad, angry, surprised, neutral)  
- ✅ Live annotated output with emotion label  
- ✅ Easy-to-use notebook setup

---

## 📁 Project Files

```
📦 Emotion_AI/
├── Copy_of_Emotion_AI.ipynb       # Main notebook
├── haarcascade_frontalface_default.xml   # Face detection model
├── emotion_model.h5               # Pre-trained CNN model (optional, if available)
├── images/                        # Optional: for testing on static images
```

---

## 📷 Input & Output

- **Input**: Live webcam feed or image input  
- **Output**: Face bounding box + predicted emotion label

Example output:
```
🙂 Detected face - Emotion: Happy
😠 Detected face - Emotion: Angry
```

---

## ⚙️ How It Works

1. OpenCV captures frames from webcam.
2. Haar cascade detects faces in each frame.
3. Faces are preprocessed (grayscale, resized).
4. CNN model predicts the emotion.
5. Prediction is displayed on the video frame.

---

## ▶️ How to Run

1. Open `Copy_of_Emotion_AI.ipynb` in Google Colab or locally in Jupyter Notebook.
2. Upload `haarcascade_frontalface_default.xml` (required) and `emotion_model.h5` (if training not included).
3. Run all cells.
4. Grant webcam access if prompted.
5. Observe live predictions.

---

## 📦 Requirements

Install dependencies:

```bash
pip install tensorflow keras opencv-python numpy
```

---

## 📊 Supported Emotions

- Happy 😊  
- Sad 😢  
- Angry 😠  
- Surprise 😲  
- Neutral 😐  

(Add more classes with extended training if needed.)

---

## ✍️ Author

**Sai Sohan Sajja**  
AI & CV Enthusiast | [LinkedIn](#)
