# Vehicle Detection

## Discription
This project intends to develop a vehicle detection program using digital image processing technique.  The system is designed to track the vehicle position. This  proposed method is using the image processing technique. This system  consists of 4 major steps:
1) Frame differencing
2) Image thresholding 
3) Finding Contours 
4) Image dilation

##  Library used

**OpenCV-Python**: OpenCV is an excellent tool for image processing and computer vision tasks. It is an open-source library that performs functions like face detection, objection tracking, landmark detection, and much more.

**NumPy**: NumPy is a Python library used for working with arrays. It also has functions for working in the domain of linear algebra, Fourier transform, and matrices.

**Matplotlib**: Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. Matplotlib makes easy and hard things possible, interactive figures that can zoom, pan, update, visual style and layout.
**Time**: provides a function for getting local time from the number of seconds.

**Gspread**: It enables you to easily pull data from Google spreadsheets into Data Frames and push data into spreadsheets from Data Frames. Gspread is a Python API for Google Sheets. Features: Google Sheets API v4. Open a spreadsheet by title, key or URL. Read, write, and format cell ranges.

**Cvlib**: A simple, high-level, easy-to-use open-source Computer Vision library for Python.
Developed with a focus on enabling easy and fast experimentation. Keras(deep learning library) inspired it.

## Execution Steps:


1.	We import our libraries, cv2, NumPy, time, matplotlib etc.
2.	We declare some variables like width_min(minimum width), height_min(minimum_height), offset(minimum error), count(initially, we advise it 0, and then it is increased) and set the position of a line.
3.	We make a list named detec; if anything is detected, it gets appended.
4.	We make a function find_center of a rectangle made on a vehicle after detecting and returning the centre points of a rectangle in the x and y direction.
5.	We extract or open video from our system using videocapture in OpenCV.
6.	Then we use one algorithm in cv2, known as a subtractor, to subtract the background of our object in the video.
7.	We run a loop to read video (as we know, video is a set of collections of frames) and for performing functions.
8.	We use cvtColor to convert colour to greyscale to increase accuracy, and then we store that frame in a variable named grey and blur that image by using GaussianBlur to reduce size.
9.	Then we use one function dilate for broadening an image by using a specific structure element that also determines the shape of the pixel.
10.	 We use getStructuringElement and MORPH_ELLIPSE to process images based on image shape; each pixel of the image pixel is adjusted based on the value of other pixels in its neighbourhood.
11.	We use the morphologyEx method that gives black white phase in the backend shown in the video and then by findContours used to count the number of objects.
12.	Then we make a function named enumerate for making rectangles on vehicles after detecting and putting text on the rectangle(VEHICLE COUNT: ) and putting a red circle in the centre of the rectangle.
13.	We also print the count down on our terminal as Output.
14.	In the final step, we release all frames, and by using destroyAllWindows, we remove all windows after completing all tasks.

</br>
</br>
</br>
</br>
<p align="center"><img width="490" alt="image" src="https://user-images.githubusercontent.com/72460920/186565101-e3022c8f-7e65-4336-85cf-fd080ec8feec.png"></p>
<p align="center"><img width="483" alt="image" src="https://user-images.githubusercontent.com/72460920/186565151-3c1e7628-c208-4cc2-9b92-ee09af1e12b6.png"></p>
<p align="center"><img width="480" alt="image" src="https://user-images.githubusercontent.com/72460920/186566432-ec38816d-0bad-43b7-aa0c-b35f5825af80.png"></p>
<p align="center"><img width="483" alt="image" src="https://user-images.githubusercontent.com/72460920/186566545-38a307a7-0040-4d38-8e55-3e8ec1830dc5.png"></p>
<p align="center"><img width="484" alt="image" src="https://user-images.githubusercontent.com/72460920/186566589-77dc3492-fc32-4e6f-9181-7ed9f233978f.png"></p>
<p align="center"><img width="481" alt="image" src="https://user-images.githubusercontent.com/72460920/186566628-7bb3a1ca-d290-40f6-ae5a-effbb451e767.png"></p>
<p align="center"><img width="477" alt="image" src="https://user-images.githubusercontent.com/72460920/186566663-7830f46b-33c7-4e73-a1e1-eb975edf23bb.png"></p>
<p align="center"><img width="478" alt="image" src="https://user-images.githubusercontent.com/72460920/186566695-bc94bd52-8de3-41bd-9307-660eadfde1e6.png"></p>
<p align="center"><img width="483" alt="image" src="https://user-images.githubusercontent.com/72460920/186566724-add661cf-7088-46a5-8362-8ce7cfa84d34.png"></p>


</br>
</br>







![Screenshot (242)](https://user-images.githubusercontent.com/72460920/186479785-1901df45-7b33-461c-a3eb-7f42be6abfcc.png)

</br>
</br>


https://user-images.githubusercontent.com/72460920/186481704-7a2cecb1-9eaa-4abd-bbba-438a342b84d7.mp4





