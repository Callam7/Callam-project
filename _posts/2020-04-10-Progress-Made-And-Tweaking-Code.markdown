---
layout: post
title:  "Progress Made & Tweaking Code"
date:   2020-04-11 1:18:04 +1200
categories: General
---

During my research around the utilization of ajax and json, I have learned that an ajax call and a json encode needs to be initiated in order for the
 data to be displayed in real-time. To do this, I created a seperate file called gauge_data.php that sets up the sql query and the json encode this way
  the ajax call can refer to this file in order to start pulling data into the graph. I have also created two other files for connection purposes, one being
   connect.inc.php and the other being error.html.php, both of which deal with connection issues and setting up connections to the server host as well as
    the database.
	

As a result of this, I have managed to get the Gauge chart to display data in real-time and also have it semi-synced with the choosen devices
 payload output rate. The query will allow the graph to limit its display to the latest payload output only, thus further semi-syncing the graph to the c02 devices.
 Seeing as currently no staff or students are at the Polytechnic building, the three devices' payloads in a way are a good reflection of their ppm responses based on the
 environment conditions that they are in:

 <img src= "{{site.baseurl}}/assets/Images/device1.PNG" alt = "gauge1">
 The first chart is showing the payload output of c02_02, of which is currently set to output every minute and is the device currently still online.
 As seen here, the chart indicates that there are consistent low levels of c02 mainly being produced between 390 and 450 indicating that there is noone currently present at the building 
 but it's still responding to low levels of c02.
 
  <img src= "{{site.baseurl}}/assets/Images/device2.PNG" alt = "gauge2">
This chart is displaying the last payload output that the c02_01 device had produced, seeing as it has not produced any new payloads for over a month.

 <img src= "{{site.baseurl}}/assets/Images/device3.PNG" alt = "gauge3">
The same story applies to c02_03, as the last output indicates that the room was heavily crowded with people during a considerably humid day.

However, I have also discovered that only one c02 device is still sending out data and has remained connected during lockdown, whereas the 
 remaining 2 devices have not produced a payload for over a month. This is both a positive and a negative, as on one hand I am able to have a responsive graph using the currently
 still operating c02 device (labeled as c02_02 within the TTN) which will provide an excellent means of testing. But on the other hand, with only one device remaining online it will proove 
 difficult in future in case we wish to expand upon the project.