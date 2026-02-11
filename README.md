# Blood Group Detection Using Fingerprint

## Overview
This project focuses on detecting human blood groups from fingerprint images using Deep Learning models.  
The goal is to provide a non-invasive, fast, and accurate method for blood group prediction using fingerprint patterns.

This system uses hybrid CNN + RNN architectures for feature extraction and classification.

## Project Highlights

- Developed hybrid deep learning models for blood group prediction
- Used CNN models: ResNet50, MobileNet, EfficientNetB0
- Used RNN models: LSTM, GRU
- Trained on 22,000+ fingerprint images
- Achieved high accuracy
- Compared performance of multiple models

---

## Models Used

- ResNet50 + LSTM
- MobileNet + GRU
- EfficientNetB0 + GRU

CNN extracts fingerprint features and RNN improves classification accuracy.

---

## Tech Stack

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

---

## Dataset

- Fingerprint image dataset
- Total Images: 22,239
- Classes:
  - A+
  - A-
  - B+
  - B-
  - AB+
  - AB-
  - O+
  - O-

Dataset split:
- Training set
- Validation set
- Test set

Images were preprocessed using OpenCV.

---

## Model Architecture

Workflow:

Fingerprint Image  
→ CNN (ResNet50 / MobileNet / EfficientNet)  
→ Feature Extraction  
→ RNN (LSTM / GRU)  
→ Dense Layer  
→ Blood Group Prediction  

---

## Results

The performance of different models is shown below:

| Model                 | Train Accuracy | Validation Accuracy  | Test Accuracy  |
|-----------------------|----------------|--------------------- |----------------|
| ResNet50 + LSTM       |  96.04%        |     71.67%           |    72.28%      |
| MobileNet + GRU       |  92.75%        |     68.03%           |    72.20%      |
| EfficientNetB0 + GRU  |  52.48%        |     63.14%           |    64.06%      |

ResNet50 + LSTM achieved the best performance with highest test accuracy of 72.28% .


---

## Project Structure

blood-group-detection-using-fingerprint/


├── Resnet_lstm.ipynb

├── Mobilenet_gru.ipynb

├── EfficientNetB0+gru.ipynb

├── README.md
