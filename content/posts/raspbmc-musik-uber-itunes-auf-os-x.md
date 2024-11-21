---
title: "RaspBMC Musik über iTunes unter OS X"
date: "2013-04-14"
tags: 
  - "airplay"
  - "itunes"
  - "music"
  - "osx"
  - "raspberry-pi"
---

Wer einen Raspberry Pi mit RaspBMC besitzt, kennt vielleicht das Problem: Musik von iTunes zum Pi über Airplay senden funktioniert nicht.

Bei mir war das so unter OS X 10.8.3 mit einem MacBook Pro Early 2011 über WLAN. Es ging mit iPhone, aber nicht von iTunes über den Mac. Deaktivieren von IPV6 hat das behoben:

> **networksetup -setv6off Wi-Fi**

Das in das Terminal eingeben, mit Passwort bestätigen und los geht es!
