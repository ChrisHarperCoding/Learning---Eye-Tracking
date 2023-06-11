# Learning - Eye Tracking



Project Name: EyeTracker



Description: An application that uses computer vision to track user's eye location and displays it in an interactive window.



Dependencies:



Python 3.8+
OpenCV
Dlib
NumPy
PyQt5



To easily check and install the dependencies:



Create a requirements.txt file in the project directory and list all the required packages:



opencv-python==4.5.4.58
dlib==19.22.0
numpy==1.21.2
PyQt5==5.15.6




Open a terminal (Command Prompt on Windows, Terminal on macOS or Linux) and navigate to the project directory using the cd command. 



Replace path/to/project with the actual path to the project folder:



cd path/to/project




Ensure Python 3.8 or higher is installed on the system. The installed version can be checked by running:



python --version



or



python3 --version




If Python is not installed or the version is lower than 3.8, download the latest version from the official website: https://www.python.org/downloads/



It is recommended to create a virtual environment for the project to isolate its dependencies. To create a virtual environment, run the following command:



python -m venv venv



or



python3 -m venv venv




Activate the virtual environment:
On Windows:





venv\Scripts\activate




On macOS or Linux:



source venv/bin/activate




The terminal prompt should now display (venv) at the beginning, indicating that the virtual environment is active.



Install the dependencies listed in the requirements.txt file by running:



pip install -r requirements.txt




This command will automatically check, download, and install the specified versions of the packages in the virtual environment.



With these instructions, a virtual environment with all the required dependencies for the project can be set up. It is important to keep the virtual environment activated. To deactivate the virtual environment, simply run:



deactivate



--------------- 



File Structure:



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
