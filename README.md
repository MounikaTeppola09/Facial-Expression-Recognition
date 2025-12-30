# Facial Emotion Recognition using MobileNet

## Deployed using GitHub Pages - https://mounikateppola09.github.io/Facial-Expression-Recognition/

## Overview

This project implements a **real-time facial emotion recognition system** that analyzes live webcam video to identify human facial expressions. Using **OpenCV**, the system detects faces in each video frame, preprocesses the detected regions and passes them to a **pre-trained MobileNet-based deep learning model** for emotion classification.

The model predicts one of eight emotion categories `Angry, Contempt, Disgust, Fear, Happy, Sad, Surprise and Neutral`and displays the predicted emotion directly on the video stream. By leveraging the lightweight **MobileNet architecture**, the application achieves efficient inference suitable for real-time use. The project demonstrates an end-to-end computer vision pipeline, combining face detection, image preprocessing, deep learning–based inference and real-time visualization.

---

## Model Details

- **Architecture**: MobileNet (Transfer Learning)
- **Framework**: TensorFlow / Keras
- **Saved Model**: `20_epochs_mobilenet_reloaded.keras`
- **Training Epochs**: 20
- **Input**: Face images extracted from video frames
- **Output**: Emotion class probabilities

---

## My Contributions (Group Project)

- Integrated and verified the pre-trained MobileNet model within the existing real-time inference pipeline
- Reviewed image preprocessing steps (resize, normalization, input shape) with the training configuration
- Checked and corrected emotion label mappings to ensure predictions were displayed accurately
- Stabilized the OpenCV–TensorFlow real-time inference loop
- Assisted in validating webcam capture, face detection, prediction display, and clean exit handling

---

## Features

- Real-time facial emotion detection via webcam
- Lightweight MobileNet architecture for fast inference
- Haar Cascade–based face detection
- Live emotion label display on detected faces
- Deployed frontend using GitHub Pages

---

## Setup Instructions

1. **Create a virtual environment:**
    ```bash
    conda create -n facial python=3.10 -y
    conda activate facial
    ```

2. **Install dependencies:**
    ```bash
    pip install tensorflow opencv-python
    ```

3. **Run the application:**
    ```bash
    python main.py
    ```
---

## Files

### `main.py`
This script runs the real-time facial emotion recognition application. It uses OpenCV to capture video frames from the webcam and detects faces using a Haar cascade classifier. Detected faces are preprocessed and passed to the MobileNet model for emotion prediction.

### `mobilenet.ipynb`
This Jupyter Notebook contains the training and evaluation code for the MobileNet-based emotion recognition model. It details data preprocessing, model training, and saving the trained model as `20_epochs_mobilenet_reloaded.keras`.

---

## Usage Notes
- Press `ctrl + q` to quit the application during runtime.
- Ensure your webcam is connected and accessible.

---

## Requirements
- Python 3.10
- TensorFlow
- OpenCV

---

## Troubleshooting
- **No webcam feed:**
  - Ensure your webcam is properly connected and accessible.

- **Missing model file:**
  - Verify that `20_epochs_mobilenet_reloaded.keras` exists in the correct directory.

- **Errors related to OpenCV or TensorFlow:**
  - Reinstall the dependencies using the command: `pip install tensorflow opencv-python`.
 


