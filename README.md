AI-powered-attendance-with-facial-recognition
AI-powered attendance with facial recognition, emotions, gender and age detection. Securely stored in Excel.

# introduction:
Automated attendance systems play a crucial role in various domains, and image recognition has emerged as a powerful tool for enhancing these systems. 
Our project focuses on leveraging image recognition for accurate gender and age detection in attendance capture, aiming to streamline and improve the efficiency of traditional attendance processes.

#Methodology:
* Data Capture:
  - Utilizes the takeImages function to capture facial images.
  - Associates each image with a unique code and user details.
  - Implements a Haar cascade classifier for real-time face detection.

* Data Storage:
  - Saves captured images and user details in a CSV file.
  - CSV file named "StudentDetails.csv" serves as a repository for code-to-name mapping.

* Training Phase:
  - Utilizes the TrainImages function to train a LBPH face recognizer.
  - Associates facial images with respective user codes.

* Real-time Recognition:
  - The recognize_attendance function identifies users during runtime.
  - Utilizes pre-trained models for gender and age predictions.

* Display and Recording:
  - Displays real-time results including user information and demographic predictions.
  - Appends results to an Excel file, "Attendance_Record.xlsx," ensuring a comprehensive attendance record.



it powered by using AI model and python code

# requirements library:
-----------------------
import os
import csv
import cv2
import cv2.face
import datetime
import time
import pandas as pd
import numpy as np
from PIL import Image
from threading import Thread
import tensorflow as tf
from tensorflow.keras.models import load_model



--> to store it use these codes in terminal: 
----------------------------------------------

pip install opencv-python

pip install pandas

pip install numpy

pip install Pillow

pip install tensorflow



# important note: 
------------------

donot forget to change paths in the code 

some files bigger than 25MB so I uploaded it to my google drive and u can access it from this link: 
https://drive.google.com/drive/folders/1Bm9p3JMH8Ndf-5z9HAbh3Q3CrnuEQf3s?usp=sharing

after downloading every thing in this link attach files to project folder 


#Block Diagram:
---------------
![image](https://github.com/Eng-Kyrolos-Ehab/AI-powered-attendance-with-facial-recognition/assets/106453561/ca3fcca2-6d7d-4d4d-b235-4e4fcb040354)

