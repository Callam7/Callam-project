---
layout: post
title:  "Updating Graphs and Finishing Tasks"
date:   2020-06-05 1:18:04 +1200
categories: General
---

Once I have managed to get the gauge chart to display and output the Device/dev_id correctly, I then
learned that the conversion was incorrect. After some testing, I decided to go on site and inspect the actual datatype
of the payload field in our database.

<img src= "{{site.baseurl}}/assets/Images/dataTypeInspection.PNG" alt = "Inspect">

I discovered that there was no real need to convert anything at all as the datatype was formatted as a varchar(256), of which
is simply the data in plain text. Therefore, I only needed to place the following variable call:

````
foreach($posts as $row)
	{
	   $v = intval($row['payload']);
	}
header('Content-type: application/json');
echo json_encode($v);
````

This in turn has allowed for the correct payloads to display for each device, with a bit of editing to the setInterval timer so that
the graph simulates real-time data display. Once I had fixed up the functionality of the graph, I then went ahead to improve upon the aesthetics
of the overall user interface. It wasnt too complex as I did not want to overshadow the functionality with flashy designs, I simply did some basic CSS styling around
the menu drop down select object so that the menu would be a bit more interactive. 

<img src= "{{site.baseurl}}/assets/Images/newInterface.PNG" alt = "Interface">


My original idea was to incorperate a responsive design using bootstrap and ajavscript, however, that had interfered with the ajax
call and the json data retrieval. I did also find some odd payload outputs for each device within the database, of which I raised some concerns
about to the other team members: 

<img src= "{{site.baseurl}}/assets/Images/payloadOutputErrors.PNG" alt = "Weird Payloads">

However, based upon the dates that each reading had been outputted, these concerns did not seem too critical at the time.

After the gauge graph had been edited, I went on to alter the CarbonGraph within the room-sensors repo so that it would contain the
correct query statement as well as the correct payload conversion. This in turn had allowed the graph to display the seven day data
readings of co2_01 with the correct payloads.

<img src= "{{site.baseurl}}/assets/Images/carbonLevelsOnline.PNG" alt = "OnlineCarbon">

Below is the highest, lowest, and average readouts of the co2_01 device's payloads over the course of a week.
<img src= "{{site.baseurl}}/assets/Images/overallStats.PNG" alt = "Stats">

Once I had confirmed that this was functioning correctly, I informed the people working on the room-sensors branch and created a new
branch with a merge request to be tested on the development server. 

<img src= "{{site.baseurl}}/assets/Images/newRequest.PNG" alt = "Request">

While I am waiting on the merge requests to be completed, I have also been looking through some data files within each repo to ensure that
we have sufficient documentation before everything is then deployed.


