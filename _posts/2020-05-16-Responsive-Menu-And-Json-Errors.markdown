---
layout: post
title:  "Responsive Menu And Json Errors"
date:   2020-05-15 1:18:04 +1200
categories: General
---

As a quick update, I have now managed to figure out how to implement the request parameter into the main file.
However, after some preliminary testing I have learned that this chunk of code does not necessarly respond to anything, and
have instead shifted it into the gauge_data json fetch file. 

   <img src= "{{site.baseurl}}/assets/Images/switchAndDropdown.PNG" alt = "switcher">


Currently, I have modified the display and menu so that the gauge chart will be more fluent without any hardcoded or repeated 
values. However, I have found that I need to modify the json file so that more than one device payload can display once a certain 
id is selected. Furthermore, I will need to modify the drafted documentation so that it has instructions on the gauge setup that
coincides with the implemented code. At the moment, I cannot carry out testing as our TTN is down so only the last payloads
that were loaded for all three devices can be accessed.