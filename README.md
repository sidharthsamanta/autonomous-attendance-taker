# autonomous-attendance-taker
a autonomous attendance taker, built on python3. It uses the face detection and image processing library openCV.

Motivation
-------------------------------------------------
  Taking the class or office attendance is very time consuming and its complexity increases with increse in the person count. So we can
deploy an AI technique to make this process easier. This is called Object Detection and to be more presized Face Detection or Recognisition.
Here we have to deploy a web camera at entrance with sufficient light. The machine (or the algorithm) will read the video and detect the face
in realtime. 


General Information
-------------------------------------------------
  Libraries
  -----------------------------------------------
  1. Numpy
  2. Pandas
  3. openCV

There are two python scripts. i.e. setup.py and autoAttend.py
  


Instructions
-------------------------------------------------
  setup.py
  -----------------------------------------------
    Here you can
      1. Reset the data and database
      2. Train the machine (Add new person)
      3. Test the camera
      4. Test the recognization
      
    For first time use:
      1. call camera(), to test the cam working properly
      2. For an external camera, change VideoCapture value 0 to 1 everywhere. **cam=cv2.VideoCapture(0)** 
      3. call reset(), to clean all the data and image database
      4. call train(), to take sample images of the person (Student or Employee)
        i. train in sufficient light
        ii. avoid presence of any other person in the background
        iii. to train place the camera at the exact place where to be deployed
      5. call recognize(), to check the face detection with name
      
  autoAttend.py
  -----------------------------------------------
    You just have to call the start() to initialize the process, and press "q" to stop the process.
    
    
Data
-------------------------------------------------
  There are two data file in csv format.
    i.e. roll.csv (holds the student name and index no information) and attendance.csv (holds the index no and attedance information.
  
Betterment Possibilities
-------------------------------------------------
  1. Removing any student
  2. single function to change camera input value
  3. backup checkpoints
  4. deployment of DBMS to store data
  >> You are free to modify and implement new concepts to the framework
  
Author's Note:
-------------------------------------------------
  I have tried to provide a detailed step by step description in the code itself by using comment line. For a better understanding 
start reading (functions) from the bottom. And for any mistakes and suggentions please let me know. Thank you

#Happy Coding :)
   
 
      
