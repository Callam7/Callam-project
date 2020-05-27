---
layout: post
title:  "Registering And Updating A Device"
date:   2020-05-24 1:18:04 +1200
categories: General
---

After going into level two, I was able to go and retrieve one of our c02 sensors from the Otago Polytechnic
site so that I could update it to sync its payload readings to the new roomsensors app and database.

To do this from my home workspace, I needed to consult the documenation that we have established within the roomsensors
repository of which contains all necessary instructions in setting up an Adafruit device. I then logged into the TTN page
and accessed the new op_roomsensors application page.

<img src= "{{site.baseurl}}/assets/Images/roomSensorOp.PNG" alt = "opsensor">

After that, I followed the documentation to ensure that the device would be registered correctly. The main difference with
 this setup is that I needed to ensure the device would have a specific id and device EUI so that it will be easier to sync up
 to the database as it is registered with those details.
 
<img src= "{{site.baseurl}}/assets/Images/deviceRegister.PNG" alt = "register">

Once the device has been registered, I then grab the session keys and place them in the c02sensor arduino file so that when
the device begins reading out its payload, it should send a signal to the gateway server. I confirmed that the payload was correct by first
running it on the Arduino IDE serial monitor:

<img src= "{{site.baseurl}}/assets/Images/co2UpdateConfirm.PNG" alt = "update">

Unfortunatly the device could not be seen within the TTN server, so I decided to test the devices range by going round my neighbour hood
block to ensure that it could get a signal outside. However, I soon discovered that the gateways we have setup around the city does not
reach my area, so therefore I would need to see if it is sending a signal at all by taking it on site.

<img src= "{{site.baseurl}}/assets/Images/noFlyZone.PNG" alt = "zone">

It maybe possible that there is something wrong with the device itself, but I would need to carry out further testing to proove that
theory.

