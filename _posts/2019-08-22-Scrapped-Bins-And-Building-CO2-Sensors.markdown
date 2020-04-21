---
layout: post
title:  "Scrapped Bins And Building CO2 Sensors"
date:   2019-08-22 1:18:04 +1200
categories: General
---

Unfortunately due to a lack of communication with the design school clients, 
 we had no choice but to scrap the project altogether as we need to be able to use the Arduino boards
 to build future projects.
 
However, we have recieved a new inquiry from our client, Neville, as he wishes to have us build Carbon
Dioxide (CO2) sensors for the Polytechnic. These will detect the ideal room temperatures in each lecture room, 
as well as the general CO2 levels being emitted within each one. I have decided to take on this task as I am in need of
 contributting more activly to the IOT/Sensors team. In order for me to fully grasp how to wire and program a CO2 Sensor,
 I had taken the liberty of locating the Data Sheet that Relates to the CO2 sensors we have in supply. This way I can better 
 understand which wires would need to connect to what as well as which ones are irrelavent to the scope of the project. The Data Sheet is located
  within our nodes repository under a branch named "CO2", as I did not wish for the file to be lost within the folder hierarchy we have set up.
  
The purpose of the Data Sheet is that displays the general schematics of the Sensors, what level of voltage it requires in order to function,
 and data tables that displays the expected output of the sensors and the product parameters. 
 
<img src= "{{site.baseurl}}/assets/Images/productParameters.PNG" alt = "Data Sheet">

<img src= "{{site.baseurl}}/assets/Images/productOutput.PNG" alt = "Data Table">

Furthermore, I located a schema to aid me in identifying what each wire is mean to be used for, as the wiring does
 not exactly line up well with the pines on the microchip.
 
<img src= "{{site.baseurl}}/assets/Images/CO2-schema.jpg" alt = "CO2 Schema">

For now, I have managed to build, or rather italicize "Frankensteined", a prototype of the CO2 sensor. This will be subject to change over time
 once I have done further research around the use of it and how to set up it's code.
 
<img src= "{{site.baseurl}}/assets/Images/CO2First.jpg" alt = "CO2 ProtoType">

