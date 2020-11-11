---
layout: post
title:  "Eye Tracking Test And Image Recognition"
date:   2020-08-12 1:18:04 +1200
categories: General
---

Today I have successfully tested the functionality of the eye tracking feature, as the infared sensors
 can track the iris of the eye. The values decrease when ever the iris of the eye is not visable to the IR sensor,
  and increases when the iris is visable. As seen below, the values fluctuate between 400 and 600, whereas the other values
   are simply me testing the IR sensors against my desk and the tip of my finger.
   
   <img src= "{{site.baseurl}}/assets/Images/redSensor.PNG" alt = "red thing">


Currently, I have yet to determine how to apply this finding to the servos and motors. In the meantime, I have been
 carrying on with the OpenCV research via testing out image recognition of which I will use as a segway into using glyph recognition
  as the primary driving tool for the robot. During the researching process, I have learned from such resources
 as [this link](https://docs.opencv.org/master/db/d28/tutorial_cascade_classifier.html) that OpenCV with any tracking function requires
 the use of Haar feature-based cascade classifiers. These haar cascades are needed to capture the shape values of certain objects being detected by the camera's frame, and the
  OpenCV library tool allows for developers to manipulate those values for use in an application.
  
In order for me to carry out this research further and to begin testing its application use, I will need
 to obtain a web camera for testing purposes as well as a small camera to attach to the head.