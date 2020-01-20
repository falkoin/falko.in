+++ 
draft = false
date = 2020-01-20T12:13:45+01:00
title = "Enabling additional languages for spell checking in Sublime Text 3"
tags = ["sublime text 3", "spell checking"]
categories = ["solutions"]
+++
I often use Sublime Text 3 for creating LaTeX documents. When doing so I really need spell checking for my texts to avoid producing gibberish. Fortunately that feature is already included, only dictionaries have to be added to support you preferred language. 

[Here](https://www.sublimetext.com/docs/3/spell_checking.html) you can find basic information on how to achieve that from the official homepage.

Unfortunately it wasn't self explanatory to me. To get new dictionaries working, go to [https://github.com/titoBouzout/Dictionaries](https://github.com/titoBouzout/Dictionaries), select the language you are looking for and make sure to download the **raw** version. If you just save the link via right click you will save the GitHub page and not the raw file. Place the **.dic** and **.aff** files in *Packages/User/*
and follow the instructions from the official site.

Credit goes to **mara**, who answered this question on [stackoverflow](https://stackoverflow.com/a/26315954/4583482)