---
title: "OS X MATLAB \"java.lang.OutOfMemoryError: Java heap space\""
date: "2013-03-07"
categories: 
  - "tech"
tags: 
  - "java"
  - "matlab"
  - "osx"
---

Beim Arbeiten mit Matlab in Kombination mit großen Videodateien (200 Hz einer Casio Exilim ZR-Serie) kam es bei mir häufiger zu der Fehlermeldung:

> java.lang.OutOfMemoryError: Java heap space

Die Fehlermeldung hängt mit dem Speicher zusammen, dem Java zur Verfügung steht. Um welchen Speicher es sich genau handelt, kann ich nicht genau sagen.

Um herauszufinden wieviel Speicher Java in Matlab zurzeit zugesichert bekommt, tippt man folgendes in die Kommandozeile von Matlab:

> java.lang.Runtime.getRuntime.maxMemory

Will man den zugesicherten Speicher erhöhen (Standard ist 192 MB), so geht man in die Einstellungen und findet unter dem Punkt **Allgemein** einen Unterpunkt **Java Heap Memory**. Dort kann man einen Regler bis 256 MB schieben (Matlab R2012a, OS X 64). Will man den Speicher weiter erhöhen, muss man selbst Hand anlegen. Eine Anleitung hierfür findet sich [hier](http://www.mathworks.de/support/solutions/en/data/1-18I2C/).

Ich habe mich für eine pragmatische Lösung entschieden und mein Video in kleine Stücke geteilt und nacheinander abgearbeitet.
