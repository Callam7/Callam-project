---
layout: post
title:  "Spring Loaded Lock Orokanui Prototype"
date:   2019-09-20 1:18:04 +1200
categories: General
---

I have finished building the spring loaded latch prototype by attaching the lock to a piece of scrap wood, 
this way the spring lock will be secure enough for use. The main idea is to place the car sensor inside the hole that is pre-drilled into the 
client's gate so that when someone pulls on the lock the sensor will indicate that it is open, but when the lock applies pressure to the sensor it will indicate that it is locked. 
In order for this to work, I have very carefully brute forced a Philips head screw into the side of the scrap wood so that it will not only hold the sensor in place but will also still apply 
a working current to the Arduino overall. This proved difficult as the drill had "twisted" the wood on the inside making it very challenging to get the screw drilled in. 

 <img src= "{{site.baseurl}}/assets/Images/LatchA.jpg" alt = "Latch">

 <img src= "{{site.baseurl}}/assets/Images/LatchB.jpg" alt = "AltLatch">

However, it appears as though I have managed to get a circuit going even though I did a poor job of the Philips head screw. 
For testing purposes, I utilized the already established code used for the latch lock prototype to test out the spring prototype. As you can see below, it functions perfectly with/without being bolted in place.

 <img src= "{{site.baseurl}}/assets/Images/Shut.jpg" alt = "Gate Shut">
	The blue LED indicates that the gate is shut/locked.
	
 <img src= "{{site.baseurl}}/assets/Images/Open.jpg" alt = "Gate Open">
	While as the red LED indicates that the gate is open/in use.

I will be using this on a different Arduino chip in order to send actual data through to the Orokanui Web Application, similar to the idea used for sending data from the CO2 sensor to the loRA server.
