---
layout: post
title:  "Switch Statements & Draft Documentation"
date:   2020-05-02 1:18:04 +1200
categories: General
---

This task has proven to be a vast challenge on its own, as the more I expand my knowledge around ajax calls and php
 the more complicated the task becomes. I have tried to implement a switch case method into the main file as a way to respond to the drop down menu,
  of which should allow the program to behave dynamiclly. This however is not the case, as although I have managed to get the drop down to somewhat respond
   if a selection is made, it will only load the c02_02 device payload and consistently redraws the pre-loaded value once selected twice:
   
   <img src= "{{site.baseurl}}/assets/Images/menuGauge.PNG" alt = "gaugeMenu">
   
As you can see, even though I have selected the c02_01 device, it continues to display the payload outpout of c02_02 seeing as c02_01 is 
still currently offline and its last payload was 1970ppm not 402ppm. Be it as it may, this has made some small level of progress as I now need to
 know how to utilize the request parameters into the query so that the menu will respond correctly with the switch statement.
 

On another note, as I am aware that the current semester is coming to a close very shortly, I have drafted up documentation on the switch method branch 
that at least explains how to create the gauge chart and what files/methods need to be utilized in order to gain a response from the database. This way, I at least have
 some documentation pre-prepared in case I somehow get my task completed before the semester ends as I will need to write up instructions on how to deploy the chart system into
  the iotsensors web application, as well as how to update it when new devices have been created.
  