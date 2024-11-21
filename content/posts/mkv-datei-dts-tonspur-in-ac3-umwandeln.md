---
title: "MKV Datei: DTS Tonspur in AC3 umwandeln"
date: "2013-01-07"
categories: 
  - "tech"
tags: 
  - "osx"
  - "video"
  - "windows"
---

Manche Streamer können Videodateien mit DTS Tonspur nur wiedergeben, wenn die Anlage am digitalen Ausgang hängt. Wenn das aber, wie bei mir, nicht der Fall ist, wird das Ganze einfach ohne Ton abgespielt. Um das Problem zu umgehen, kann die Tonspur in das AC3 Format umgewandelt werden.

Unter OS X findet sich die komfortable Lösung [Remux](http://www.macupdate.com/app/mac/35968/remux). Damit kann man einfach innerhalb des MKV-Container die Tonspur umwandeln, ohne händisches De- und Remuxen. Mit gedrückter ALT-Taste kann man vorher eine Kopie der Tonspur anfertigen, so dass beide Spuren erhalten bleiben.

[Bildschirmfoto_2013-01-07_um_09](/images/bildschirmfoto_2013-01-07_um_09-02-59-scaled1000.png)

Unter Windows habe ich früher eine etwas umständlichere Prozedur benutzt, die allerdings genauso erfolgreich sein sollte.

Man benötigt die Programme [MKVextract](http://sourceforge.net/projects/mkvextractgui-2/), [eac3to](http://www.homecinema-hd.com/eac3tougui_en.html) und [MKVmerge/MKVtoolnix](http://www.videohelp.com/tools/MKVtoolnix).

Zunächst extrahiert man die DTS Tonspur mit MKVextract. Anschließend wandelt man sie in das gewünschte AC3-Format mittels eac3to und fügt die Spur abschließend wieder der MKV-Datei hinzu (MKVmerge). Dabei kann gewählt werden, ob die DTS-Tonspur behalten oder verworfen werden soll.
