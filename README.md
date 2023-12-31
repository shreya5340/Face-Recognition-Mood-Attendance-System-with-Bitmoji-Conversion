# Face Recognition Mood Attendance System with Bitmoji Conversion

## Overview

The *Face Recognition Mood Attendance System with Bitmoji Conversion* is an innovative Python-based application that leverages computer vision and machine learning technologies to automate attendance tracking while capturing the mood of each individual. This project offers three main functionalities:

1. *Face Recognition Attendance*: The system recognizes individuals in real-time using face recognition algorithms. It identifies registered faces in front of the web camera and logs their attendance automatically, eliminating the need for manual check-ins.

2. *Facial Emotion Detection*: The system detects the facial emotions of the recognized individuals in real-time. Utilizing a pre-trained Convolutional Neural Network (CNN) model, it accurately predicts emotions such as happiness, sadness, anger, and more.

3. *Bitmoji Conversion*: After recognizing an individual and detecting their mood, the system converts their face into a personalized bitmoji image. This fun and creative feature add an enjoyable touch to the attendance logging process.

## Tech Stack

The Face Recognition Mood Attendance System with Bitmoji Conversion uses the following technologies and libraries:

- *Python*: The application is developed in Python, taking advantage of its versatility and extensive libraries for computer vision and machine learning.

- *openCV*: OpenCV is a powerful computer vision library that provides tools for image and video processing, facial recognition, and emotion detection.

- *face_recognition*: The face_recognition module is utilized for face detection and recognition. It accurately recognizes registered individuals based on facial encodings.

- *Convolutional Neural Network (CNN)*: The CNN models are used for real-time emotion and gender detection. The models are trained on a large dataset of facial emotion and gender images, allowing it to predict emotions and gender accurately.

- *matplotlib*: This library is used to analyse the models that were trained.

- *scikit-learn*: A Python library for machine learning that provides a comprehensive set of tools for data preprocessing, modeling, and evaluation.


## How It Works

1. *Face Recognition Attendance*: The system captures video feed from the web camera using OpenCV. It then uses the face_recognition module to detect and recognize faces in real-time. By comparing the facial encodings of detected faces with registered individuals, the system logs their attendance.

2. *Facial Emotion Detection*: After recognizing a face, the Haarcascade frontal face classifier is used to detect facial regions of interest. The detected regions are passed through the trained CNN models, which predict the individual's emotion and gender. The predicted emotion is displayed alongside the detected face.

3. *Bitmoji Conversion*: Once the face and emotion are detected, the system overlays the bitmoji corresponding to their gender and emotion on their faces.

## Installation

1. Clone the repository:

git clone https://github.com/shreya5340/Face-Recognition-Mood-Attendance-System-with-Bitmoji-Conversion

2. Download the facial emotion detection model:

https://github.com/shreya5340/Face-Recognition-Mood-Attendance-System-with-Bitmoji-Conversion/blob/main/model.h5

3. Download the gender detection model:

https://drive.google.com/file/d/1yn0Oe9X9k4HqLMgDvr5QslcWyc_FyVTb/view?usp=drive_link

4. Download the emotions dataset (Optional):

https://www.kaggle.com/datasets/jonathanoheix/face-expression-recognition-dataset

5. Download the gebder dataset (Optional):

https://www.kaggle.com/datasets/maciejgronczynski/biggest-genderface-recognition-dataset

## Usage

1. Run the main script:


ATTENDANCE.ipynb


2. The web camera feed will open, and the system will start recognizing faces, displaying their emotions, and generating personalized bitmoji images.

3. The system will automatically log attendance for recognized faces in a designated CSV file.

4. To exit the application, press q.

## Note

- The attendance register will be updated only after the ATTENDANCE.ipynb file is terminated completely.
- Name of the attendance register will be saved by the date on which it will be run with CSV file extension.

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
- scikit-learn
- matplotlib
- os

---
