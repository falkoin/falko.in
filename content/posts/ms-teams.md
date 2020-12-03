+++ 
draft = false
date = 2020-12-03T09:26:26+01:00
title = "Enabling EpocCam with MS Teams"
tags = ["MS Teams", "EpocCam"]
categories = ["macOS", "solutions"]
+++

For work I use the communication platform [MS Teams](https://www.microsoft.com/de-de/microsoft-365/microsoft-teams/group-chat-software), which makes having a webcam kind of mandatory.
Since I used to work with my laptop in clamshell mode, I wasn't able to use the internal webcam.
That's when I discovered [EpocCam](https://www.elgato.com/de/epoccam), a software, which makes it possible to use a smartphone as webcam.
Using your smartphone is not only pretty convenient but has also very good quality when compared with a standard webcam.

At some point MS Teams stopped recognizing EpocCam after an update.
After a quick web search I found a [thread](https://answers.microsoft.com/en-us/msteams/forum/msteams_tfb-msteams_tfmac/microsoft-teams-mac-os-client-is-not-recognizing/d9e863be-d9a4-4d03-a4b8-1b5c7df58828) with a solution.
Unfortunately I have to apply this solution every time I update MS Teams, but at least it works.


Here is the solution:
```
sudo codesign --remove-signature "/Applications/Microsoft Teams.app"
sudo codesign --remove-signature "/Applications/Microsoft Teams.app/Contents/Frameworks/Microsoft Teams Helper.app"
sudo codesign --remove-signature "/Applications/Microsoft Teams.app/Contents/Frameworks/Microsoft Teams Helper (GPU).app"
sudo codesign --remove-signature "/Applications/Microsoft Teams.app/Contents/Frameworks/Microsoft Teams Helper (Plugin).app"
sudo codesign --remove-signature "/Applications/Microsoft Teams.app/Contents/Frameworks/Microsoft Teams Helper (Renderer).app"
```

Use these command in the terminal when MS Teams is closed. The next time it starts up you have to give some permissions again, which is quite inconvenient.