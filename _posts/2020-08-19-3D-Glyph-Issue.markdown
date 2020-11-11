---
layout: post
title:  "3D Success And Glyph Problems"
date:   2020-08-20 1:18:04 +1200
categories: General
---

Yesterday, I had managed to finally get a prototype head printed out using glow in the dark ABS. This was
 quite time consuming as the printer had been clogged with hardened PLA, ABS, and other plastic material. This was causing
  the gears within the nozzle from extruding the material correctly. However, this small issue has given me the benefit of teaching
   myself how to troubleshoot and maintain the Dremel printer in hopes of not running into a similar issue in future.
   
<img src= "{{site.baseurl}}/assets/Images/protoType.jpg" alt = "abs">

Although this was a success, I cannot use this module as the final product as the ABS is far too fragile to work with, as the
 simple action of using a drill head on it fractures the general structure of the head shell. Therefore, I have insteed printed a
  final product using gray PLA filament on a slow print speed as to prevent any clogging or spoiling.
  
<img src= "{{site.baseurl}}/assets/Images/newFace.jpg" alt = "pla face">

As a bonus, I have managed to printout a prototype eye barrel using red PLA, of which I have found to be very sturdy
 in terms of structural integrity. Originally, I was going to hold the eye barrel in place using the small pins used to solder jumper wires 
 on a breadboard, however, as they seem to be too lose I decided to insteed go with the smallest screw heads but will use support structure in the eyes to
  prevent any damage to them and the head.
  
  After I had this done, I went on to work with the glyph recognition software. I have, however, found it challenging as 
  the code seems to crash after detecting the glyph for a few seconds. The code was a modified example that I found from this [resource](https://rdmilligan.wordpress.com/2015/07/19/glyph-recognition-using-opencv-and-python/).
  This is disappointing as the hope for this application was that the camera would scan the shape and pattern of a glyph and drive towards it based on the distance from the robot's echo sensors
  and data read out. The shapes would be on various colored paper and in various patterns, as the glyph recognition is meant to be
  able to scan a QR code such as the example below:
  
<img src= "{{site.baseurl}}/assets/Images/QR.PNG" alt = "qr">

In theory, if the glyph recognition can scan a QR code, then it gives reason to believe that it should scan other patterns of a 
similar sequence. I have made a decision that if this issues persits after debugging the code and reevaluating its logic, I will look
towards an alternative for the driving mechanism such as face tracking.

  