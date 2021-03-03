+++ 
draft = false
date = 2021-03-03T09:17:33+01:00
title = "Changing handbrake's automatic aspect ratio detection"
tags = ["handbrake","video"]
categories = ["solutions"]
+++
From time to time I do screen recordings, which include a PowerPoint with an aspect ratio of 4:3. When encoding these video files with [handbrake](https://handbrake.fr/) it tries to be smart about it and automatically detects the aspect ratio of the video, which usually results in a cropped video.  
But there is an easy fix for that. Go to the picture tab and change the cropping option to 0 in all directions.
![Handbrake Screenshot](/images/handbrake.png)

