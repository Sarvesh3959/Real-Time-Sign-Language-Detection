# Real-Time Sign Language Detection

This project is a real-time sign language detection system developed using a combination of machine learning models and computer vision techniques. It is designed to recognize and interpret sign language gestures in real-time, making it a useful tool for facilitating communication between hearing-impaired individuals and others.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Dataset Creation](#dataset)
- [Model Training](#model)
- [Output](#output)

## Introduction

The primary objective of this project is to capture hand signs via a webcam, label these images, and then train a deep learning model to recognize various sign language gestures. The model is then tested in real-time to assess its accuracy and effectiveness.

This project follows these steps, which guides you through the entire process from data collection to real-time prediction.

## Features

- **Image Capture**: Capture hand sign images using a webcam or any image source.
- **Image Labeling**: Use the `labelImg` tool to label the captured images.
- **Model Training**: Using pretrained model `ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8` to accelerate the development process and improve the accuracy of our sign language detection system. This model is a variant of the MobileNetV2 architecture, optimized for real-time object detection.
- **Real-Time Detection**: Implement real-time hand sign detection using the trained model.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Sarvesh3959/Real-Time-Sign-Language-Detection.git
   cd Real-Time-Sign-Language-Detection

## Dataset Creation

In this project, it is crucial to create a custom dataset tailored to the specific hand signs you want the model to recognize. A well-labeled dataset is essential for training a machine learning model to accurately classify and predict sign language gestures. By creating your own dataset, you ensure that the model is trained on the exact gestures and variations that are relevant to your application. For convenience labeled dataset is uploaded in `Tensorflow/workspace/images` directory for 1-9, A-Z, and some basic words hand signs.

**Creating the Dataset with LabelImg**:
Capture Hand Sign Images: Use the provided `Image Collection.ipynb` script to capture images of different hand signs. Ensure that the images are clear and represent the sign language gestures accurately. These images will be saved in the `Tensorflow/workspace/images/collectedimages` directory.

**Label the Images**: Use the LabelImg tool to label each image with the corresponding sign label. Labeling involves drawing bounding boxes around the hand signs in each image and assigning them the correct label.

- Launch LabelImg.
- Load the images from the `Tensorflow/workspace/images/collectedimages` directory.
- For each image, draw a bounding box around the hand sign and assign a label (e.g., "A", "B", etc.).
- Save the labeled files in the `Tensorflow/workspace/images/collectedimages` directory.
- Double-check the labeled data for accuracy. Mislabeling or inaccurate bounding boxes can lead to poor model performance.

## Model Training

Use the provided `Train and Test.ipynb` script to train the model and for real time sign language detection.

## Output

Output of this project is shared in this repository.
