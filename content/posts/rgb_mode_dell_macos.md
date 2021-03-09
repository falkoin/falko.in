+++ 
draft = false
date = 2021-03-09T14:34:50+01:00
title = "Fixing color/sharpness issues with external displays on macOS (RGB/YCBCR)"
tags = ["display issues"]
categories = ["macOS", "solutions"]
+++
The first time I connected my BenQ XL2730 display to my MacBook the image looked very blurry and I started googling the issue.  
I found out that the issue is related to the color-mode a display is identified with, either RGB or YCBCR. Usually you want your display to be connected with RGB color, but my BenQ was fixed on YCBR without any option to changing it. After more research I found a script to modify some system files so the display is forced into RGB mode. That worked and I was happy.  
With my current Dell display (U2515H) I had the same issue, except I was able to switch to RGB, but then the colors turned purple/greenish. I tried to apply the same patch as I did with the BenQ, which nowadays was way harder, because you have to temporarily disable [SIP](https://support.apple.com/de-de/HT204899), but without success.  
Luckily I found this [updated script](https://gist.github.com/ejdyksen/8302862), which can be used without any changes to SIP or even rebooting the system. Now everything is fine again.