---
title: "ISO aus VIDEO_TS Ordner erstellen"
date: "2012-12-12"
categories: 
  - "tech"
tags: 
  - "osx"
  - "video"
---

Um unter OS X 10.8 ein ISO Image aus einem VIDEO\_TS Ordner zu erstellen, wird nur folgender Befehl im Terminal benötigt:

> hdiutil makehybrid -iso -o Image.iso /input\_path

Image.iso bezeichnet in diesem Beispiel den Namen, /input\_path den VIDEO\_TS Ordner.
