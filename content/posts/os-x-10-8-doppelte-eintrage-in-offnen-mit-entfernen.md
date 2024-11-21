---
title: "OS X 10.8 Doppelte Einträge in \"Öffnen mit\" entfernen"
date: "2012-12-01"
categories: 
  - "tech"
tags: 
  - "osx"
---

Unter OS X 10.8 müllt sich "Öffnen mit" im Kontextmenü nach und nach durch mehrfache Einträge der selben Programme zu. Um dem Einhalt zu gebieten hilft folgender Terminalbefehl:

> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/  
> LaunchServices.framework/Versions/A/Support/lsregister -kill -r -domain local  
> \-domain system -domain user

Mit diesem Befehl werden die Launchservices aktualisiert.

Leider finden sich dort immer wieder mal Mehrfacheinträge ein, so dass man diese Prozessur ab und zu wiederholen muss. Meine Beobachtung ist, dass dies bei Updates betroffener Anwendungen passiert.
