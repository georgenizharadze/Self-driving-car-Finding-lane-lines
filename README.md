## Finding Lane Lines on the Road

In this project, I use the tools I have learned about in Udacity's Self-driving Car Nanodegree lesson to identify lane lines on the road. I develop my pipeline on a series of individual images, and later apply the result to a video stream (which is really just a series of images). 

The tools I use are color selection, region of interest selection, grayscaling, Gaussian smoothing, Canny Edge Detection and Hough Tranform line detection. I piece together a pipeline to detect the line segments in the image, then average/extrapolate them and draw them onto the image for display. Once I have a working pipeline, try it out on the video stream below.

This repository contains the following files:



### Reflection

This has been new type of learning and exercise for me. I had to learn a mathematical representation of an image, the relevant python and openCV libraries and functions and the common image processing operations. I managed to identify lane lines successfully. The output of my code was not always steady and the red lines flickered and momentarily branched out to sides from time to time. Not sure if this would be a problem for a real self-driving car or not. I subsequently adjusted two parameters - increased the HoughLinesP "threshold" parameter and decreased the "min\_line\_length" parameter. This improved the result to some extent. 