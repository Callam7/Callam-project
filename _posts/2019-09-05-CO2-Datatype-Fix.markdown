---
layout: post
title:  "CO2 Datatype Fix"
date:   2019-09-05 1:18:04 +1200
categories: General
---

The CO2 sensor has been set up with the adafruit feather Arduino chip and is currently sending data to server, 
although it is not displaying the correct data at the moment. I have found that the float datatype that was 
being assigned to the adjustedADC variable needed to be converted to a byte first then to an int datatype. 
This way the loRA server would be spitting out the correct CO2 level in hexdecimal format, 
 however, I have to prevent the data from rounding up from its original decimal value. 
 
 Therefore, I have managed to adjust the CO2 sensor so that it is reading correctly with the fixed values to the loRa server network. 
 The delay reaction time needed to be reduced slightly in order for the sensor to be given enough time to 
 adjust to its environment. I will need to solder (not weild) an antenna in order for it to gather range within a 
 certain area (i.e. similar to how the range works on the loRa server gateways we recieved). 
 
 <img src= "{{site.baseurl}}/assets/Images/SampleAntenna.jpg" alt = "Antenna">
