---
layout: post
title:  "Further Errors and Merge Requests"
date:   2020-05-18 1:18:04 +1200
categories: General
---

After some investigation into the console side of the c02 graph, I have discovered that for some strange
reason the gauge_data file does not seem to be sending/recieving any data whatsoever. 

<img src= "{{site.baseurl}}/assets/Images/nullError.PNG" alt = "error">

For this to properly function, I have continued to research around json encoding within a function to
determine if my code is actually achieving its functionality in the first place.

Meanwhile, I have been reviewing a few merge requests and performed a code review to ensure that no code was deleted
without the owner's knowledge of doing so. First off, I reviewed the below merge request that involved the deletion of the 
.gitignore file: 

<img src= "{{site.baseurl}}/assets/Images/merge.PNG" alt = "merge">

I then pointed out that the main purpose of a gitignore is to prevent unwanted files from being committed in the first place:

<img src= "{{site.baseurl}}/assets/Images/mergeComment.PNG" alt = "mergeCommenting">

The owner had then diverged from deleting the gitignore file as its usage was standard practise in using git.

Secondly, I recently did a code review of another project student's code to ensure that there were no conflicts:

<img src= "{{site.baseurl}}/assets/Images/merger2.PNG" alt = "mergers">

I ran through their code and comments to ensure that there was no conflicts to the original. I then commented on certain lines of
code to be sure that the owner wished to delete them, as they were reference to an object she had previously created.

<img src= "{{site.baseurl}}/assets/Images/approved.PNG" alt = "approval">
