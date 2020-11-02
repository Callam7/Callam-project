---
layout: post
title:  "Open CV Research And Raspberry Pi"
date:   2020-08-06 1:18:04 +1200
categories: General
---

Now that I have some level of idea for what hardware I require based off of my inventory list, I have begun to carry
out some much needed research into the software application of the robot. I have found that in order to have some level of a 
one-to-many device relationship structure, I need to incorporate the use of a Raspberry pi model, of which will have it send out commands to
all motors and devices.

Therefore, I briefly drew up a diagram of what I believe is how the raspberry pi should operate once implemented correctly:

   <img src= "{{site.baseurl}}/assets/Images/diagramPi.PNG" alt = "unit diagram">
   
For the movement portion of the robot, I will be using the python library Open CV with the raspberry pi pi-camera to measure the distance of an given object,
and have the robot "chase" the object until they reach a certain distance from them. The distance will be determined through a series of echo sensors attached to the base of the 
tracks so that it will know not to hit anything.

    <img src= "{{site.baseurl}}/assets/Images/echoSensors.jpg" alt = "echo">


For starters, I will be going through the Open CV application to determine how the library should be installed and how to interact with it. Thankfully, as I have 
done such papers as Data Science/Machine Learning and Object-Oriented Systems Development, I am more than familiar with the concept of object orientated programming, as well as
the application use of python and Open CV. Thus this will make it all the more smoother to establish a working idea rather than spend too much time on researching.

With this familiarity, I will research the following possible applications for Open CV:
	1. Color Tracking
	2. Object Tracking
	3. Face Recognition & Tracking
	4. Glyph Recognition
	5. Facial Expression & Image Recognition
	
This way, I will not only have a few options on what to use, but if I can apply these successfully I could make the raspberry pi camera feature "multi-functional".
