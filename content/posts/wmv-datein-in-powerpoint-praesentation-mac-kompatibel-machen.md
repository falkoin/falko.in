---
title: "WMV-Datein in PowerPoint Präsentation Mac-kompatibel machen"
date: "2017-04-18"
---

Kurz und knapp: Ich habe eine Präsentation bekommen, in der WMV-Dateien eingebettet waren und mein Mac diese nicht abspielen konnte. Microsoft empfiehlt mir an dieser Stelle einen Codec zu kaufen. Eine bessere Lösung, die ich gefunden habe, war folgende:

Die PowerPoint Präsentation kopieren und in .zip umbennnen und dann mit dem Programm "[The Unarchiver](https://itunes.apple.com/de/app/the-unarchiver/id425424353?mt=12)" (mit der hauseigenen Mac-Extrahierungssoftware hat es nicht funktioniert) entpacken. Dort finden man nun alle Mediendateien und kann diese mit seinem bevorzugten Programm (bei mir [ffmpeg](https://ffmpeg.org/)) in ein kompatibles Format umwandeln und anschließend in der Präsentation ersetzen.
