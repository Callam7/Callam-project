---
layout: post
title:  "Raspberry Pi OS And Interfacing"
date:   2020-09-01 1:18:04 +1200
categories: General
---

As of this post, the servo is able to turn the prototype head as well as support it's general structure. This offers a great deal of optimism
 in terms of what the neck mount will have the potential to achieve once constructed. In the mean time, I have begun working on flashing the rasbian OS to
 the raspberry pi using the Rasbian SD installer.
 
 <img src= "{{site.baseurl}}/assets/Images/raspberry1.PNG" alt = "1 raspberry">
 
During the installation process, I have been making careful note of any documentation needed for the raspberry pi, as well as other programming tools,
 in case anything goes wrong. Once the installation was complete, I attempted to get the pi to communicate with the arduino, however, it does not seem to
 accept any values from the python IDLE commandline as the arduino serial cannot read any format other than bytes. Therefore, I had to
 modify the test code of the OpenCV face tracker so that the string values are converted into utf-8 encoding, thus allowing for the string to be readable in
 byte formats.
 
 
This has resulted in doing some further testing as I have yet to explore the idea of having the head pan and tilt based on the person's face position.
Furthermore, as the eye tracking method seems to not respond well with the raspberry pi and its power limitations, I have made a decision to utilize the 
face tracking code so that I can send the arduino the x y coordinates that the python IDLE reads out and use them as directional values for two servos. Thus creating a functional head
 that moves based on the user's face position.

 <img src= "{{site.baseurl}}/assets/Images/headMount.PNG" alt = "head mounter">
