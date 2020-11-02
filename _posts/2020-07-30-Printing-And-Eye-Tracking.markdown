---
layout: post
title:  "Printing Problems And Eye Tracking Research"
date:   2020-07-30 1:18:04 +1200
categories: General
---

Today I have managed to print out a prototype of the head shell model using the glow in the dark ABS filament
 within the dremel 3-D printed. This took a bit of time as I have found that ABS is quite fragile and requires certain settings to maintain the general structure of
 the print. Therefore, once I have managed to work with the prototype a bit I will be using a stronger solution for the master build, either PLA or PA will be used for the "primary" 
 parts of the body and structure.
 
   <img src= "{{site.baseurl}}/assets/Images/protoType.jpg" alt = "abs sucks">
   
There was a lot of support structure to dig away at, so I may reevaluate the concept of even having support structure for the entire build. I have also learned that the dremel 3-D
printer requires a lot of monitoring and maintanence in order to successfully print out any model whatsoever, therefore I will work on some form of documentation for the print settings 
around certain 3-D parts just for future reference.


Now that I have a prototype established, I have begun researching around the eye tracking mechanism for the head turning mechanic. In my research, I have found a arduino enthusiast who
has created a eye tracking model that has two infared sensors clipped onto novalty glasses. This tracks the white of her iris and has LED lights follow along
with her eyes' movements.

[Here is what she has worked on](https://create.arduino.cc/projecthub/H0meMadeGarbage/eye-motion-tracking-using-infrared-sensor-227467)

Because there is some level of complexity to this, I have made a note to keep all research links within a README markdown
file under Studio 5, this way any documented content that may seem too complex to follow will have a reference to their origin. 
Furthermore, I will also create a stationary or "inventory" list to ensure I know what hardware I have avaliable to me.

As this user implements the use of LEDs for her eye tracking model, I will replicate a portion of that and 
use two LEDs that will indicate if the user's eye has shifted in one direction to the next, as well as get the infared sensors
to communicate with a servo motor.
