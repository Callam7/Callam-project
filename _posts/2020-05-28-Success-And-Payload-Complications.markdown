---
layout: post
title:  "Success And Payload Complications"
date:   2020-05-27 1:18:04 +1200
categories: General
---

After some consistant testing, I have now managed to get the gauge chart to have a response
as data can now be recieved and displayed in-line with the selected devices.

<img src= "{{site.baseurl}}/assets/Images/responseSuccess.PNG" alt = "Success">

The problem was that I needed to have the #Device.val() assigned to the dev_id inside the ajax calls.

Now that I have data being displayed, I then went to the Polytechnic site to access the database we are using
to store all device payloads/outputs. Once I had access via following our documentation with the ppk file, I then saw
that the device I had updated can now send through data to the things database.

<img src= "{{site.baseurl}}/assets/Images/co2Sending.PNG" alt = "sending">

<img src= "{{site.baseurl}}/assets/Images/dataSending.PNG" alt = "datasend">


However, I had a bit of concern around why one specific device was registered under two different application ids, as this
could possibly cause issues with other applications in future.

<img src= "{{site.baseurl}}/assets/Images/strangeDBIds.PNG" alt = "idstrange">

Be it as it may, I then went to change my query statement in the gauge_data.php file in order for the updated devices to be displayed.
However, I later learned that the new payload output is sending through as an integer not as a string, of which I now would need
to update the payload conversion in order to get accurate data readings.

<img src= "{{site.baseurl}}/assets/Images/payloadTrouble.PNG" alt = "trouble">

As you can see below, the updated chart is now showing obsurd payload outputs:

<img src= "{{site.baseurl}}/assets/Images/strangePayloadOutput.PNG" alt = "outputerror">

For now, I will need to update my documentation, as well as all branches with code commenting in order to acoid confussion and
to allow our dev team to begin creating docker containers to deploy the gauge chart. Furthermore, it seems I will also need to update the
payload conversion within the CarbonGraph we used for the showcase display.

<img src= "{{site.baseurl}}/assets/Images/graphAlter.PNG" alt = "alterGraph">




