---
title: "pygame mit Python 3.4 und MacPorts auf dem Mac"
date: "2015-02-19"
categories: 
  - "tech"
tags: 
  - "pygame"
  - "python"
---

Möchte man [pygame](http://pygame.org) auf dem Mac installieren, muss man schnell feststellen, dass die aktuelle Version auf der Homepage noch auf Basis von Python 2.7 läuft. Mit wenig Aufwand kann man sich selbst eine Version auf Python 3.4 basierend erstellen.

- Zunächst installiert man [Python](https://www.python.org/) 3.4, falls man das eh nicht schon getan hat
- Wer XCode oder die XCode Developertools noch nicht hat, der wird [hier](https://developer.apple.com/xcode/downloads/) oder im Mac App Store fündig.
- Anschließend besorgt man sich [MacPorts](https://www.macports.org/) (zur Installation einiger Pakete) und [XQuartz](http://xquartz.macosforge.org/landing/) (grafische Darstellung)
- Zuletzt lädt man noch diese [Datei](http://dudeslife.com/images/scale_mmx64.c) herunter (angepasste Datei zur Installation von pygame)

Wenn die oben genannte Software installiert ist, startet man ein Terminal und installiert ein paar nötige Pakete:

> sudo port install mercurial

System zur Versionskontrolle - wird später für pygame benötigt.

> sudo port install libdsl libsdl\_image libsdl\_mixer libsdl\_ttf portmidi
> 
> sudo port install smpeg

Abhängige Pakete installieren.

> cd yourPreferedDownloadDirectory/
> 
> hg clone https://bitbucket.org/pygame/pygame

Download der aktuellen Version von pygame.

> cd pygame/src
> 
> cp yourPreferedDownloadDirectory/scale\_mmx64.c .

Austausch einer Datei, damit die Installation klappt.

> pip3 install yourPreferedDownloadDirectory/pygame

Installation von pygame. Unter Umständen erscheint nun eine Fehlermeldung, die folgendes enthält:

> 'X11/Xlib.h' file not found #include <X11/Xlib.h>

Ist dies der Fall, müsst ihr noch einen letzten Befehl ausführen:

> sudo ln -s /opt/X11/include/X11 /usr/local/include/X11

Linkt X11 an die richtige Stelle. Um zu überprüfen, ob alles geklappt hat startet ihr nun Python:

> python3.4

Importiert das Modul pygame:

> import pygame

Falls jetzt keine Fehlermeldung erscheint, hat alles geklappt und pygame steht zur Verfügung.

Die meisten Informationen stammen nicht von mir, sondern wurden nur von mir zusammengesetzt. Hilfreiche Informationen fand ich auf [DudesLife.com](http://dudeslife.com/blog/2014/programming/installing-python-3-3-3-pygame-on-os-x-mavericks/) und dem [Blog von shinriyo](http://d.hatena.ne.jp/shinriyo/20140117/p2).

_Hinweis: Diese Anleitung wurde mit OS X Yosemite (10.10.2) und Python 3.4 getestet._
