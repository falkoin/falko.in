---
title: "OS X Mission Control Lag Fix"
date: "2013-05-27"
categories: 
  - "tech"
tags: 
  - "osx"
---

Ich hatte heute ein mysteriöses Problem mit der Animation von Mission Control, das auch schon mal unter Lion auftrat. Damals habe ich noch neu installiert, weil es mich so genervt hat. Es ist zwar rein kosmetischer Art, aber ich bin gut darin, mich in so etwas reinzusteigern.

Es äußert sich durch eine ruckartige Animation beim Aufruf von Mission Control. Der Hintergrund bleibt flüssig animiert, aber die Fenster springen vom Anfang bis zum Ende der Animation, kein flüssiger Übergang dazwischen.

Diesmal bin ich auf eine Lösung im Forum von [MacRumors.com](http://www.macrumors.com) gestoßen. Dieser Bug lässt sich ganz leicht beheben und zwar, indem man das Benchmark [Xbench](http://xbench.com/) herunter lädt und es einmal ausführt. Man soll wohl die Option "Thread Test" deaktivieren, da es sonst abstürzt. Nach dem Durchlauf sind alle Animationen wieder flüssig wie eh und je.

![Picture of Xbench](/images/bildschirmfoto-2013-05-27-um-17-05-16.png)  
Thread Test besser deaktivieren

Wie der Durchlauf eines Benchmarks die Performance der Animation wiederherstellt ist mir ein Rätsel. Froh darüber bin ich dennoch.
