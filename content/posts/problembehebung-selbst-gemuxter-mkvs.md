---
title: "Problembehebung selbst-gemuxter MKVs"
date: "2012-11-14"
categories: 
  - "tech"
tags: 
  - "osx"
  - "video"
---

Ich hab früher öfters Tonspuren extrahiert, umgewandelt und verschoben. Dazu war das Programm [mkvtoolnix](http://www.matroska.org/node/62) perfekt geeignet.

Leider hatte ich bei meinen aktuellen Versuchen keinen Erfolg. Mein Streamer hat entweder keinen Ton abgespielt oder ist einfach abgestürzt. Mit folgenden Einstellungen bin ich allerdings zum Ziel gekommen:

- Programm starten
- Mit **add** Datei auswählen
- Tonspurreihenfolge ändern mit **up** und **down**
- Gewünschte Tonspur markieren
- In **General track options** Sprache auswählen
- Standardsprache setzen (**Default track flag** auf **yes**)
- **Extra options** auswählen und unter **Compression** die Option **none** wählen
- Zum Umwandeln **Start muxing** anklicken

![1s](/images/1s-scaled1000.jpg)
![2s](/images/2s-scaled1000.jpg)
![3s](/images/3s-scaled1000.jpg)
![4s](/images/4s-scaled1000.jpg)
