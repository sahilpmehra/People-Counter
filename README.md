# People-Counter
This program counts incoming and outcoming people, who cross the hall. 
  I found many video tutorials on how to count the inflow and outflow of people but couldn't find any code examples sp, I decided to write a little program which does so.
  I used OpenCV and Python 2.7
  So, begining you need install all dependensies:
   #pip install datetime
   #pip install imutils
   #pip install opencv-python
   
   For running program write in command line 
   #python PeopleCounterMain.py
   
   If you want to change the video or set stream from rtsp camera, change line
   camera = cv2.VideoCapture("test2.mp4") 
   
   This example uses mechanism computer the absolute difference between the current frame and
   previous frame, so I compare two frame and if changes exist i find where. If biggest area is more than 
   12000, I draw rectange around object which has been changed, if less then contour is too small, ignore it.

  
