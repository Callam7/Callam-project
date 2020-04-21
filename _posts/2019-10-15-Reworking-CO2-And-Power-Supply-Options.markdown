---
layout: post
title:  "Reworking CO2 And Power Supply Options"
date:   2019-10-15 1:18:04 +1200
categories: General
---

I have begun fixing the CO2 sensor data, however, there was an inherent need for some assistance behind 
the mathematics of the CO2 calculations, as I am not very adept at maths in general. Once we had fixed the equation to calculate the CO2 levels, I then referred 
to the datasheet about switching from Analog 0 to serial RX and TX. This has proven with some assistance that we can get far more accurate CO2 readings 
than we had previously. Furthermore, I have managed to reuse some old power supplies used for previous projects in order to power the adafruit microchips. 

 <img src= "{{site.baseurl}}/assets/Images/newSupply.jpg" alt = "new">

Therefore, we now have a functioning CO2 sensor with a power supply and antenna attachment, the only variable left is to figure out the sleeper dog agent that will power 
cycle the sensor when it reaches a certain point. However, I will need to go through each adafruit feather chip to ensure that they are all soldered correctly as I have found 
that the current one keeps disconnecting from the server.

 <img src= "{{site.baseurl}}/assets/Images/fixedSupply.jpg" alt = "fix">


However, I have recently found that the current power supplies will be insufficient in powering the CO2 sensors. 
Therefore, we have decided through deep discussion that they should instead be plugged in at all times to enable an actual sufficient power 
supply that does not require manual interference. Thus I will disregard the sleeper dog agent as it will not be required for this type of set up.
