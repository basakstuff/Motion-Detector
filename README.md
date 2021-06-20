# Python Motion Detector
A Python program that can detects moving objects with webcam and log their entry and exit time to/from the camera


# Requirements
- Python 3.5 or above
- Camera or Video file
- Install OpenCV or `pip install opencv-python`
- Install Bokeh library or `pip install bokeh`

# How it Works?
The script "motion_detector.py" utilizes the openCV library to capture video from the default webcam of the loacal machine. and we basically store the first frame, which ideally would capture the static background, and then check every coming frame captured from the camera to see if the difference (delta) in all pixels surpasses the set threshold. If it does, we draw rectangular contours on the frame to indicate where the detected objects are.

After we are able to successfully detect the moving objects, the next step is to record the entry and exit points in time and plot a time series with my second script- "plotting.py". The time series chart is plotted with the bokeh library and we also enable hovering effect to show the time stamps. The only thing left to do is to fine tune the parameters such as the threshold in order to make the detection more accurate.

# Usage

* Before you execute the project, please cover your webcam and remove the cover once your webcam starts and you can see some video recording windows on your desktop.

* You will see four different windows on your screen.

* Color Frame: Which detects the different objects

* Current Frame: Which detects the human face

* Delta Frame*: Which compares the current situation the with the initial situation

* Threshold frame* - for identification of an object

![1](https://user-images.githubusercontent.com/25417307/122678810-f8b68700-d1f0-11eb-851f-d2bd5a669851.png)
![2](https://user-images.githubusercontent.com/25417307/122678811-f9e7b400-d1f0-11eb-8bd4-8c2842dab145.png)


* At any moment if you want to stop, please press `q`

* A motion graph will be generated and automatically your default browser will pop-up where you can see it like this:

![3](https://user-images.githubusercontent.com/25417307/122678796-f05e4c00-d1f0-11eb-9157-525ae3ecf38f.png)





# Author 


[@Basak ER](https://www.linkedin.com/in/basaker/)
