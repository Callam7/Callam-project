---
layout: post
title:  "Face Mask, Raspberry Pi, And Face"
date:   2020-08-28 1:18:04 +1200
categories: General
---

After much consideration, I have decided to go with the use of face tracking as the head's driving mechanism
 rather than glyph recognition. However, as glyph recognition shows high applicable use, I will not be scrapping it
  completly and will insteed have it archived as an option in case the bugs can be removed.
  
The face tracking mechanism was quite simple to code, as it hsared similarities to the glyph recognition 
and object tracking code. It utilizes the haar cascade xml values to identify the location and general shape of 
a person's face, of which is then read out as data in the python IDLE serial in a utf-8 format. This raises an interesting concept, as 
this can possibly be used to send data from the python IDLE to the arduino, allowing for the servos to move and respond on the face positioning values
that are read out in the serial. If so, this will require some major testing stages in future.

While I was working on this, I have managed to get a raspberry pi 2 and an SD card to flash the rasbian OS to. This will be my main controller for the 
robot, so from this point on I will need to dedicate my time to ensuring that the pi can communicate with multipl devices via sending commands through IDLE or serial.


On a side note, I have managed to print out the face plate/mask of the head and have attached it with small screw heads.
I have also completed the eye sockets, of which is being held together via hooking in screws within the support structure of the eyes. Furthermore,
 the details of the eyes were made with white PA filament, of which has been fitted in without the use of any abrassive holding tool.
 
<img src= "{{site.baseurl}}/assets/Images/finalHead.jpg" alt = "final part">

Unfortunatly, I have had to reprint the face plate as it had fractured during the drilling process. To save time, I will reduce the settings of the print job
 and stick with one filament type for any details.
