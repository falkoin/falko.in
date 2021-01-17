+++ 
draft = false
date = 2020-12-28T12:28:32+01:00
title = "Using the command-line in macOS to resize images"
tags = ["resize", "sips"]
categories = ["macOS", "solutions"]
+++

Creating the photo section for this blog I had the need to resize many images at once. Sure enough, I didn't want to do this by hand and also found it cumbersome to create a batch process in an image manipulation program like Affinity Photo or Photoshop.

After a quick web-search I stumbled upon the tool **sips**.

```
sips -Z 2000 *.jpg
```

This command resizes all jpg files in a folder to a maximum height or width of 2000, while keeping the aspect ratio. 