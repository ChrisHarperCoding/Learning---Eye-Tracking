# Learning - Eye Tracking

Project Name: EyeTracker

Description: An application that uses computer vision to track user's eye location and displays it in an interactive window.

Dependencies:

Python 3.8+
OpenCV
Dlib
NumPy
PyQt5
File Structure:

lua
Copy code
EyeTracker/
|-- app/
|   |-- __init__.py
|   |-- main.py
|   |-- eyetracker.py
|   |-- webcam.py
|-- models/
|   |-- shape_predictor_68_face_landmarks.dat
|-- README.md
|-- requirements.txt
|-- setup.py
|-- LICENSE
Contents:

README.md: A comprehensive description of the project, setup instructions, and usage guide.
requirements.txt: A list of the Python packages required for the project.
setup.py: A Python script for installing the project's dependencies.
LICENSE: A license file, such as the MIT License, which ensures the project is legally compliant.
app/__init__.py: An empty file that indicates the app directory is a Python package.
app/main.py: The main entry point for the application, handling the UI and user interactions.
app/eyetracker.py: Contains the EyeTracker class, responsible for eye detection and tracking.
app/webcam.py: Contains the Webcam class, responsible for capturing frames from the user's webcam.
models/shape_predictor_68_face_landmarks.dat: A pre-trained model file for facial landmark detection.
Here's a brief outline of the main components and their functionalities:

main.py: This script will contain the main UI code using PyQt5. It will create an interactive window that displays the webcam feed with eye locations represented using circles. The Webcam and EyeTracker classes will be used to capture frames and track eye locations.

eyetracker.py: The EyeTracker class will use OpenCV and Dlib to detect and track the user's eye locations in real-time. It will take a frame from the Webcam class and process it, returning the eye locations.

webcam.py: The Webcam class will use OpenCV to capture frames from the user's webcam. It will provide a simple interface to start and stop the webcam, as well as retrieve frames for further processing.
