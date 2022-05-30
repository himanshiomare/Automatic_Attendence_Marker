# Automatic_Attendance_Marker
Marking attendance using face recognition.


## Problem Statement

Because of the online education, students are missing their classes and not paying attention.. So I have made this automatic attendance marking application for maininting the decorum of classes.

## Solution
1. Images will be saved in the folder.And this model will diffrentiate between the real video and photographs.It will mark present only when the live video  will match with the photo in the folder, and when it will detect photo it will show invalid.
2. After the detection the name of the student,date and time will be recorded in xl file for records.

## ML Model 
1. This  model  is trained to  differentiate between real live vdo and photographs which checks the liveliness. It will mark present only when it will detect live video and for the photos it will be invalid.
2. face-recognition package is used which has more than 99% accuracy detects face and encodes them.
3. A threshold (95%) is set. Faces above this similarity are recognized.
4. Siamese network compares the live video with the all the photos in the people folder using the cosine similarity. 

## Dependencies
To run the project make sure to install the following dependencies installed on your system.

1. OpenCV
2. flask
3. flask SQL Alchemy
4. flask-lgoin
5. Tensorflow
6. Panda
7. Keras
8. Face-recogniton

## Instructions
1. Clone the project.
2. Install all the dependencies
* `pip install -r requirements.txt`
3. Save the photos in people folder with their names
4. Reach to the directory of project folder
* `python app.py`
