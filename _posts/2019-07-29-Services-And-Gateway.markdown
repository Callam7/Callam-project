---
layout: post
title:  "Working With Services And Gateway Disassembly"
date:   2019-07-30 1:30:04 +1200
categories: General
---

Recently I found out that most of our services were down over the four week break period, and I had been tasked
 with ensuring that they are up and running. To do this, I consulted the Dev ops team to see if they could
 check that loRa server and the web temperature app was running. They found that both seemed to be working fine,
  however it was soon found that although the server used for the web app was fine, the actual app itself was not running
   at all. Luckily no data was lost as the web app still recieved its data before it stopped.
   
<img src= "{{site.baseurl}}/assets/Images/temp app stopped working.png" alt = "Web App Broken">

It was fixed later on as it turned out the python version it was running was not compatible with
 the web app and needed to be updated in order for the scripts to run correctly. 
 
I also worked on taking the current gateway we have appart so it would be prepared for the Orokanui visit
 that we have planned for next Wednesday. This was due to the decission that the gateway sensor would
 not need to be weather proofed, however, the wiring we would be using would most certainly
 need to be weather proofed as well as protected from other variable. Apart from the services running and disassembling the current
  gateway framwork, it was a very light work load for today.
 
<img src= "{{site.baseurl}}/assets/Images/Gateway frameA.jpg" alt = "framed">


<img src= "{{site.baseurl}}/assets/Images/Gateway frameB.jpg" alt = "Taken apart">


 
 
