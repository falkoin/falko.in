---
title: "OS X: Fehler bei Updates beheben"
date: "2013-05-24"
categories: 
  - "tech"
tags: 
  - "itunes"
  - "osx"
---

Bei der neuen Version von iTunes kam es bei mir zu einem Fehler (103) bei der Installation. Danach war weiterhin eine Benachrichtigung über das neue Update zu sehen, es ließ sich aber unter keinen Umständen installieren.

Die Ursache war vermutlich eine korrupte Installationsdatei. Um diese zu löschen und somit ein erneutes Herunterladen zu erzwingen, geht man wie folgt vor:

Terminal starten:

> cd /Library/Updates/

Dort nach einem Ordner suchen der in etwa so aussieht: zzzz041-9781

> cd zzzz041-9781
> 
> sudo mv iTunes\*.pkg /tmp/

Passwort eingeben und fertig. Die fehlerhaften Dateien wurden nun in das Verzeichnis /tmp verschoben. Falls sie doch nicht die Ursache waren, könnte man sie dort später wiederherstellen. Nun kann man erneut versuchen, das Update herunter zu laden und zu installieren.

Bei mir hat das so funktioniert.
