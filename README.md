# Drowsiness detection using OpenCV and Keras

This Python script uses OpenCV and Keras to detect eye states (open or closed) in real-time using a webcam. It can be used to monitor drowsiness in a person's eyes, especially for applications like driver drowsiness detection.

## Prerequisites

Before running the script, ensure you have the following installed:

- **Python**: You'll need Python installed on your system.

- **OpenCV (cv2)**: OpenCV is used for image and video processing. Install it using pip:

  ```shell
  pip install opencv-python
  pip install keras
  pip install pygame
  
## Getting Started
-git clone https://github.com/nikolozGobejiShvili/Drowsiness-detection.git

## How it Works
-The script uses Haar Cascade Classifiers to detect faces and eyes in the webcam feed.
-It then extracts the left and right eyes from the detected face regions.
-The eyes are resized, preprocessed, and fed into a trained Keras model for classification (open or closed).
-Based on the model predictions, it tracks the eye state and calculates a "score."
-If the score exceeds a certain threshold, it triggers an alarm and marks the frame as potentially drowsy.

## Customization
-You can adjust the threshold for triggering the alarm by modifying the score > 15 condition.
-The sound alarm is played using pygame with a 'alarm.wav' file. Make sure you have this sound file in your project directory
