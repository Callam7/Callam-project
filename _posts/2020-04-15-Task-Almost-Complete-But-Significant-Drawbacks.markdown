---
layout: post
title:  "Task Almost Complete & Significant Drawbacks"
date:   2020-04-16 1:18:04 +1200
categories: General
---

I have made considerable progress these past few days, as I have managed to produce a gauge chart system that allows the user to select a c02 device 
with a pre-set button. 

 <img src= "{{site.baseurl}}/assets/Images/selectGauge.PNG" alt = "buttonGauge">

However, I have come across an error in which the gauge needle value will always set to the c02_02 payload regardless of whether or not
 a different device is selected. Also the button draw methods consistently override the display real-time payloads with the ppm values that displayed onLoad
  everytime the buttons are clicked.
  

Furthermore, after a brief scheduled meeting, I have learned that the code I have produced is not up to standard as it has hard coded values,
 repeative code, and as this project will most likely be used again when we create more c02 devices it would be inenifficent to constantly add the
 same code over and over just to output the selected device. Therefore, I have made a complete roll back of my code in the master branch so that only the active device is selected
 as I rather would have clean code working than a almost completed task with below average code robustness. I have also listed down comments in my repo of what it is I need
 to change, for example:

```
    What needs to be fixed:
	1. The draw method and the getData method needs to be called once without repeating code
	2. The user needs to be able to select which device to display in the gauge chart via drop down menu
	3. I need to be able to have only one query that I can use to select a device via dev_id WITHOUT creating another payload variable (i.e. $v) to display the required output
	4. The drawChart function should not override the displayed payload value with the value it was loaded with on refresh
	
```

This way, once I get some assistance with my task then others will be able to understand what I need to alter in order to get the task functioning in an 
 efficient and clean way.
 