# **Finding Lane Lines on the Road** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

In this project we need to detect lane lines in images using Python and OpenCV.  OpenCV means "Open-Source Computer Vision", which is a package that has many useful tools for analyzing images.  

Pipeline
---
My pipeline mainly consist of ten functions which are explained below
* Start with image or frame from video clip
<img src="test_images/solidWhiteCurve.jpg" width="480" alt="Combined Image" />

* Convert the image to gray scale
<img src="test_images/solidWhiteCurve_gray.jpg" width="480" alt="Combined Image" />

* Apply Gaussian filter to remove noise
<img src="test_images/blurred.jpg" width="480" alt="Combined Image" />

* Auto Canny Edge Detection
I have come up with the auto canny edge function to get the lower and higer thresholds automatically for the canny edge detector. 
<img src="test_images/solidWhiteCurve_auto_canny_edge.jpg" width="480" alt="Combined Image" />
