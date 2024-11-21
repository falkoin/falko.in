---
title: "Automatisierung mit Shell Script (Bash) und curl"
date: "2014-01-06"
categories: 
  - "tech"
tags: 
  - "osx"
---

Bei einem Ausflug durchs Netz bin ich auf ein kostenloses Buch gestoßen, welches ich gerne haben wollte. Leider war das Buch nur in einzelnen Kapiteln zu haben und ich hatte wenig Lust 34 einzelne PDF-Dateien von Hand zu klicken. Daher habe ich ein kleines Shell Script geschrieben, mit dem das automatisch geht.

Dazu braucht man [cURL](https://de.wikipedia.org/wiki/CURL) (Client for URLs) und einen Texteditor. Hier ist es für OS X erklärt, sollte so aber auch problemlos auf Linux, etc. übertragbar sein.

![shell](/images/shell.jpg)

Das Skript basiert hauptsächlich auf einer **FOR-Schleife** die von 1 bis 34 durchlaufen wird. Die aktuelle Zahl wird an der Stelle **$(i)** eingesetzt und steht im Dateinamen für das Kapitel. Voraussetzung ist natürlich, dass das auch für alle Dateinamen gilt. In diesem Beispiel entstehen also Dateinamen von _filename1.PDF_ bis _filename34.PDF_. Der Befehl curl ist einfach für das herunterladen der Datei zuständig. Der Parameter **\-O** führt zum Speichern der Datei. Ohne -O würde nur der Inhalt der Datei wiedergegeben werden. Ausgeführt wird das Skript mit:

> sh example.sh
