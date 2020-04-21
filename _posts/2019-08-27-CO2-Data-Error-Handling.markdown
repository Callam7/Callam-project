---
layout: post
title:  "CO2 Data Error Handling"
date:   2019-08-27 1:18:04 +1200
categories: General
---

CO2 sensor is not giving out correct readings on the analog, as the connections are far too lose or interfered with other wiring to get a correct reading.
 Furthermore, it is producing incorrect analog power readings, as according to the datasheet provided it should be spitting out at least 2 volts,
 whereas it is producing well over 3.3 volts. I will need to solder it in order to get the correct readings, however the code has been reworked to match the board schematic that I had previously set up. 
 
<img src= "{{site.baseurl}}/assets/Images/Fluctuating Data CO2.PNG" alt = "Irregular Data">

<img src= "{{site.baseurl}}/assets/Images/CO2Third.jpg" alt = "faulty wiring">
 
Due to this data fluctuating in irregular rhythms, I had decided to begin soldering the wires that link to the RX-TX side of the sensor board. This way the voltage will actually travel correctly as the soldered 
 material should conduct the voltage enough to complete the circuit. However, I have found that this is not the case as after using a multimeter to check if any voltage actually travelled, the wiring that I have been
 supplied with does not actually link up to the sensor at all as the white casing around them seems faulty and has therefore interfered with the VO-Analog connection.
  
<img src= "{{site.baseurl}}/assets/Images/SolderA.jpg" alt = "solder not weild">

 
Therefore, I soldered the connections to GND, PWM and VIN as well as a pin connection VO-analog; this way I would get a more stable reading out of the sensor. 
However, have found it to still oscillate at random when left alone. Instead, I soldered pins to the actual board to get a more frequent reading, this way it would make the assembly process more simplistic
and straight forward provided it works correctly.

<img src= "{{site.baseurl}}/assets/Images/SolderB.jpg" alt = "solder working">

<img src= "{{site.baseurl}}/assets/Images/CO2Forth.jpg" alt = "CO2 Fixed">
