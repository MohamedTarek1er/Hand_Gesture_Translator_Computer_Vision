Hand Gesture Sign Language Recognition System

This project aims to bridge the communication gap for individuals who are non-verbal or have speech impairments by enabling them to communicate using hand gestures. It recognizes English and Arabic letters, numbers, and commonly used words through hand gestures and converts them into readable text, and optionally displays the output on an LCD screen or through a mobile application.

Project Overview

The Hand Gesture Sign Language Recognition System leverages Computer Vision, Machine Learning, IoT, and Mobile Development to create an interactive and inclusive platform. The system detects hand gestures using a camera and translates them into letters or words in real-time. It supports Arabic and English alphabets, digits, and some frequently used words.

Goals

Enable communication for people who are unable to speak.
Support both Arabic and English sign language.
Recognize not only alphabets and digits but also commonly used words.
Provide multi-platform output: On-screen display, IoT LCD screen, and mobile app.
Ensure accuracy, usability, and accessibility.

Technologies & Tools Used

Computer Vision
MediaPipe: For real-time hand landmark detection.
OpenCV: For image processing and camera frame handling.

Machine Learning

Collected and preprocessed gesture image data from various resources.
Trained ML models to classify hand gestures (letters, numbers, and words).
Applied data augmentation and normalization for better model generalization.

Internet of Things (IoT)

Arduino UNO & ESP8266: Microcontrollers for IoT connectivity.
LCD Display: To show the recognized gesture output for real-world hardware feedback.
Used serial and Wi-Fi communication between the model and the hardware.

Mobile Application

Developed a mobile app to allow users to:
Use the camera to detect hand gestures.
View gesture-to-text conversion.
Enable smoother communication on-the-go.

How It Works

Hand Detection: The camera captures real-time video frames. MediaPipe detects the hand and landmarks.
Gesture Classification: Extracted landmarks or image data are passed through the trained ML model.

Output Display:

The detected character or word is displayed on the desktop.
Optionally, it's sent via Wi-Fi to an Arduino-connected LCD screen for visual output.
Alternatively, it is shown directly inside the mobile app.

Dataset
Collected gesture data from:
Open-source sign language datasets.
Custom images captured using webcam and mobile camera.

Covers:

A-Z (English)
(Arabic)
0-9 (Numbers)
A few frequently used words (like "Hello", "Thank you", etc.)

Features
Supports both Arabic and English sign languages.
Works in real-time using the device's camera.
Offline capability in mobile app (depending on version).
IoT integration for external hardware output.
Modular system — each part (ML model, CV detection, IoT, mobile) can work independently.

Installation & Usage
Requirements

Python 3.x
MediaPipe
OpenCV
TensorFlow / scikit-learn
Arduino IDE
Android Studio or Flutter (for mobile app)

Run the Detection
bash
Copy
Edit
python hand_gesture_recognition.py

Upload Code to Arduino
Use Arduino IDE to flash the ESP code.
Connect LCD via I2C interface.

Mobile App
Build and run the app using Android Studio.
Camera permission required for gesture capture.

Screenshots
(Add some screenshots here of gesture detection, LCD output, and mobile app interface.)

Future Improvements

Expand dataset to support full sentence recognition.
Add voice output (text-to-speech).
Integrate chatbot or assistant for contextual responses.
Cloud syncing of results for monitoring and logging.
