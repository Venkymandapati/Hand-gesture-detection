# Hand-Tracking-using-Mediapipe

It will detect tips of hands by inbuilt camera 

## Documentation
# Hand Tracking with OpenCV and MediaPipe

This Python project demonstrates hand tracking using OpenCV and the MediaPipe library. It captures live video from the webcam and identifies and tracks hand landmarks, making it useful for applications involving hand movements.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Demo](#demo)
- [License](#license)

## Prerequisites

Before using this project, ensure you have the following installed:

- Python 3.x
- OpenCV (cv2)
- MediaPipe

You can install MediaPipe using pip:

pip install mediapipe
## Installation

Ensure that you have the necessary Python libraries installed. You can use pip to install them:

pip install opencv-python
pip install mediapipe

    
## Demo

It looks like you've provided Python code for hand tracking using the MediaPipe library and OpenCV. This code captures video from the default camera (index 0) and detects hand landmarks using the MediaPipe library. Here's a brief explanation of what the code does:

*Import necessary libraries:

*cv2: OpenCV for handling computer vision tasks.
*mediapipe: MediaPipe library for hand tracking.
Create a video capture object (cap) to access the default camera (index 0).

Initialize the MediaPipe hands module, which allows you to detect hand landmarks.

Define a class handtracking with a method subbu that takes a video capture object as a parameter.

*Inside the subbu method:

Read a frame from the camera using cap.read().
Convert the frame to RGB format since MediaPipe expects RGB images.
Process the frame to detect hand landmarks using the hands.process method.
If there are multiple hands in the frame, iterate through each hand's landmarks.
For each landmark (a point on the hand), extract its position, convert it to pixel coordinates, and print the landmark's index, and its x and y coordinates.
Draw landmarks on the image using mpDraw.draw_landmarks.
Display the annotated frame in a window named "Image" using cv2.imshow.
*The cv2.waitKey(1) function is used to display the image for 1 millisecond, allowing you to view the video feed frame by frame.

To use this code, make sure you have the necessary libraries installed (OpenCV and MediaPipe). You can also modify the code as needed to perform specific tasks with hand tracking.


## License

The code you've provided appears to be using two open-source libraries: OpenCV and MediaPipe. These libraries are generally distributed under open-source licenses. The licenses for these libraries are as follows:

*OpenCV: OpenCV is released under the Open Source Apache 2 License, which allows you to use, modify, and distribute the library freely, as long as you follow the terms of the license. You can find the full text of the Apache 2 License in the OpenCV repository or on the OpenCV website.

*MediaPipe: MediaPipe is also an open-source project developed by Google. It is released under the Apache License 2.0, which is a permissive open-source license that allows you to use, modify, and distribute the software, subject to certain conditions.

Both of these licenses are permissive and generally allow you to use the libraries in your projects without significant restrictions. However, you should always review the specific terms of the licenses for the most accurate and up-to-date information.

Please note that when using these libraries in this project, it's essential
