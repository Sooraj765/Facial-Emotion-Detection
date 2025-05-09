# EmoNet: Facial Expression Recognition using CNN and Transfer Learning

## 📌 About
EmoNet is a deep learning-based facial emotion recognition system that identifies human emotions from facial expressions. Built using Convolutional Neural Networks (CNN) and MobileNetV2 with transfer learning, the project aims to recognize 7 distinct emotions: Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise. The system is capable of real-time inference via webcam input and was developed as part of a final year university project.

## 🎯 Features
- Classifies facial expressions into 7 emotion categories
- Trained on the FER-2013 dataset
- Uses both custom CNN and MobileNetV2 architectures
- Real-time emotion prediction using OpenCV and webcam
- Includes detailed classification report and accuracy logs
- Modular code structure for training, evaluation, and inference

## 📂 Dataset
The project uses the **FER-2013** dataset:
- 35,887 grayscale images of size 48x48 pixels
- 7 emotion classes: Angry, Disgust, Fear, Happy, Neutral, Sad, Surprise
- Organized into `train/`, `test/`, and `validation/` directories

## 🧠 Model Architecture

### ✅ Custom CNN:
- 3 Convolutional layers with ReLU + MaxPooling
- Flatten → Dense (512) → Dropout
- Output: Dense (7) with softmax

### ✅ MobileNetV2 Transfer Learning:
- Pretrained on ImageNet
- Custom top layers for emotion classification
- Fine-tuned for optimized performance

## 📊 Results
- Best Validation Accuracy (Custom CNN): **56.25%**
- Best Validation Accuracy (MobileNetV2): **~42.3%**
- Classification report includes per-class precision, recall, and F1-score
- Real-time detection with ~15 FPS on CPU

## 🛠️ Installation

Clone the repository:
git clone https://github.com/yourusername/emotion-recognition-emonet.git
cd emotion-recognition-emonet
