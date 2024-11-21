---
title: "Verschlüsselt chatten mit Jabber - Detailanleitung Teil 1: OS X"
date: "2013-07-10"
categories: 
  - "tech"
tags: 
  - "encryption"
  - "osx"
  - "security"
  - "sicherheit"
  - "verschluesselung"
---

Um die Einstiegshürde für Verschlüsselung zu verkleinern gibt es nun eine Detailanleitung, wie man unter Windows/OS X/Linux mit Jabber verschlüsselt chattet. Dies ist der erste Teil, der sich mit dem Betriebsystem OS X (getestet unter 10.8 Mountain Lion) beschäftigt.

Es bietet sich der Multi-Messenger [Adium](https://adium.im/) an. Damit ist es sehr leicht möglich ein Konto zu erstellen und dieses anschließend zu verschlüsseln.

Zunächst wählt man bei Adium unter "Datei" den Punkt "Einstellungen". Dort angekommen klickt man auf den Menüreiter "Konto". Mit dem kleinen "Plus mit dem Pfeil nach unten" gelangt man zur Kontoauswahl. Dort wählt man XMPP aus. Dies ist der Standard, der von Jabber verwendet wird.

![dienstauswahl](/images/dienstauswahl.png)

Anschließend sucht man sich einen Benutzernamen aus. Zum Beispiel "MrExample23". Ein @jabber.org muss nicht angehängt werden. Im Bereich Passwort wählt man ein möglichst sicheres Passwort. Ein sicheres Passwort generiert man sich zum Beispiel so: Man wählt zwei Worte: "Rainbow", "Unicorn". Ersetzt Buchstaben durch entsprechende Zahlen (Stichwort: [1337-Speak](https://de.wikipedia.org/wiki/Leetspeak)). Also nimmt man zum Beispiel: "R41nb0w" und "Un1c0rn". Setzt diese zusammen, indem man sie mit einem Sonderzeichen verbindet und verändert die Groß- und Kleinschreibung: "r41Nb0w\_un1C0rn". Anschließend fügt man noch etwas zum Anfang oder Ende hinzu: "17$r41Nb0w\_un1C0rn". Man könnte jetzt behaupten, dass sich das kein Mensch merken kann, aber dem möchte ich folgendes entgegnen. Die beiden Worte können ja welche sein, mit denen man etwas verbindet. Für die Zahl kann das Gleiche gelten und den Rest macht man eben immer gleich, nach System.

Nun klickt man auf "Neues Konto registrieren".

![benutzername](/images/benutzername.png)

Im folgenden Fenster wählt man den Jabber-Server des [CCC](https://de.wikipedia.org/wiki/Chaos_Computer_Club) aus. Dieser verschlüsselt meines Wissen die Daten auch auf dem Server, was sonst eine Schwachstelle sein kann. Mit einem Klick auf "Neues Konto anfordern" generiert man nun ein neues Konto. Die Voraussetzung ist allerdings, dass der Benutzername noch frei ist. Zu beachten ist auch, dass Konten, die 12 Monate unbenutzt bleiben, automatisch gelöscht werden.

![serverwahl](/imaages/serverwahl.png)

Um jetzt noch die Verschlüsselung zu aktivieren, geht man im Menü "Einstellungen" in den Menüreiter "Erweitert" und wählt dort in der linken Seitenleiste den Punkt "Verschlüsselung". Dort wählt man das neu erstellte Jabber-Konto aus und klickt auf den Punkt "Neu generieren". Hiermit wird ein Schlüssel generiert, der zur Identifizierung gegenüber euren Chatpartnern dient.

![verschluesselung](/images/verschluesselung.png)

Um nun verschlüsselt chatten zu können, müsst ihr nur noch im Chatfenster auf das Schlosssymbol klicken. Die Voraussetzung dafür ist natürlich, dass der Chatpartner auch das Verschlüsseln des Chats eingerichtet hat. Wie das geht, kann man diesem ja anhand dieser Anleitung erklären.

![chatten](/images/chatten.png)

**Ausblick:**

In einem weiteren Eintrag werde ich erklären, wie das beschriebene unter Windows beziehungsweise Linux zu verwirklichen ist.

Außerdem wird es einen Artikel zu verschlüsselten Chats und mobilen Geräten geben.
