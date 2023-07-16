# Face Recognition Mood Attendance System with Bitmoji Conversion

## Overview

The *Face Recognition Mood Attendance System with Bitmoji Conversion* is an innovative Python-based application that leverages computer vision and machine learning technologies to automate attendance tracking while capturing the mood of each individual. This project offers three main functionalities:

1. *Face Recognition Attendance*: The system recognizes individuals in real-time using face recognition algorithms. It identifies registered faces in front of the web camera and logs their attendance automatically, eliminating the need for manual check-ins.

2. *Facial Emotion Detection*: The system detects the facial emotions of the recognized individuals in real-time. Utilizing a pre-trained Convolutional Neural Network (CNN) model, it accurately predicts emotions such as happiness, sadness, anger, and more.

3. *Bitmoji Conversion*: After recognizing an individual and detecting their mood, the system converts their face into a personalized bitmoji image. This fun and creative feature add an enjoyable touch to the attendance logging process.

## Tech Stack

The Face Recognition Mood Attendance System with Bitmoji Conversion uses the following technologies and libraries:

- *Python*: The application is developed in Python, taking advantage of its versatility and extensive libraries for computer vision and machine learning.

- *OpenCV*: OpenCV is a powerful computer vision library that provides tools for image and video processing, facial recognition, and emotion detection.

- *face_recognition*: The face_recognition module is utilized for face detection and recognition. It accurately recognizes registered individuals based on facial encodings.

- *Convolutional Neural Network (CNN)*: The CNN model is used for real-time emotion detection. The model is trained on a large dataset of facial emotion images, allowing it to predict emotions accurately.

- *Bitmoji API*: The Bitmoji API is integrated into the system to convert detected faces into personalized bitmoji avatars. The API uses facial features and detected emotions as input to create expressive and unique bitmoji images.

## How It Works

1. *Face Recognition Attendance*: The system captures video feed from the web camera using OpenCV. It then uses the face_recognition module to detect and recognize faces in real-time. By comparing the facial encodings of detected faces with registered individuals, the system logs their attendance.

2. *Facial Emotion Detection*: After recognizing a face, the Haarcascade frontal face classifier is used to detect facial regions of interest. The detected regions are passed through the pre-trained CNN model, which predicts the individual's emotion. The predicted emotion is displayed alongside the detected face.

3. *Bitmoji Conversion*: Once the face and emotion are detected, the system sends this information to the Bitmoji API. The API processes the input data to create a personalized bitmoji avatar reflecting the individual's facial features and mood. The bitmoji avatar is displayed alongside the individual's face.

## Installation

1. Clone the repository:


git clone https://github.com/shreya5340/Face-Recognition-Mood-Attendance-System-with-Bitmoji-Conversion


2. Download the pre-trained facial emotion detection model:

https://github.com/shreya5340/Face-Recognition-Mood-Attendance-System-with-Bitmoji-Conversion/blob/main/model.h5
## Usage

1. Run the main script:


ATTENDANCE.ipynb


2. The web camera feed will open, and the system will start recognizing faces, displaying their emotions, and generating personalized bitmoji images.

3. The system will automatically log attendance for recognized faces in a designated CSV file.

4. To exit the application, press q.

## Limitations

- The accuracy of face recognition and emotion detection depends on the quality of registered face images and the emotion detection model used.
- The bitmoji conversion may not capture all facial features or complex emotions perfectly.

## Future Enhancements

- Integrate with an attendance management system to record attendance data in a central database.
- Improve emotion detection accuracy by fine-tuning the CNN model with more diverse emotional expressions.
- Implement real-time data visualization to display attendance statistics and emotion distribution.

## Acknowledgments

- face_recognition
- opencv-python
- numpy
- csv
- datetime
- keras
- time
- tensorflow

---
