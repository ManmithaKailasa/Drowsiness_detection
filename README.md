-Drowsiness_detection
This project implements a real-time drowsiness detection system using OpenCV, dlib, and SciPy. It leverages facial landmark detection to monitor eye aspect ratio (EAR) and triggers an alarm if drowsiness is detected.

-Key Features
.Real-time Drowsiness Detection: Utilizes webcam feed for live monitoring.
.Eye Aspect Ratio (EAR) Calculation: Calculates EAR to determine eye closure.
.Facial Landmark Detection: Employs dlib's shape predictor for accurate facial landmark localization.
.Alarm System: Plays an audible alarm using winsound when drowsiness is detected.
.Configurable Thresholds: Allows customization of EAR threshold and frame count for triggering the alarm.
-Technologies Used
.OpenCV: For image processing and video capture.
.dlib: For facial landmark detection.
.SciPy: For calculating the Euclidean distance (used in EAR calculation).
.imutils: For basic image processing tasks.

-How It Works
The system works by:

Detecting Faces: Using dlib's frontal face detector to find faces in the video frame.

Locating Facial Landmarks: Identifying 68 facial landmarks using a pre-trained shape predictor.

Calculating Eye Aspect Ratio: Computing the EAR for both eyes. The EAR decreases as the eyes close.

Drowsiness Detection: If the EAR falls below a defined threshold for a certain number of frames, the system triggers a drowsiness alert (visual and audible).
-Dependencies
.opencv-python
.dlib
.scipy
.imutils

-Usage
.Install the required dependencies: pip install opencv-python dlib scipy imutils

Download the shape_predictor_68_face_landmarks.dat file (available from dlib's website or other online sources) and place it in the specified directory. Note: You will need to update the shapePredictor variable in the script to the correct path of the .dat file.

Run the drowsiness_detection.py script.

Press 'q' to quit.
