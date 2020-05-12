---
layout: post
title:  "Difficulties & Created Branches"
date:   2020-04-22 1:18:04 +1200
categories: General
---

As stated previously, I have been struggling with creating my gauge chart system as I now have to update its functionality
 so that it has robust code and produces the gauge chart dynamiclly without manuelly editing the devices.
 
For this, I have started to work on pushing new branches to my project repo as I make attempts on various methods to produce dynamiclly displayed
 data via drop down menu selection. This way I can manage my version control and show my levels of research and progress as I work on the task, seeing as 
 pushing straight to master is both inefficient and frowned upon. So far I have tried a if statement with a pre-set $_POST request variable that is then
  defined and loaded into the sql query. The initial idea was that the query would update based upon the user's selected device within the drop down menu,
   however, this has proven to be unresponsive and messy code as there is no response to the selection.
   

Despite this drawback, I have started to look into the process of using request parameters as another method of retrieving the data. This also falls into the category
 of "solving unfamiliar problems" as if I can resolve this it will reflect positivly on my project.