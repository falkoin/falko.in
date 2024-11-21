---
title: "ebay Passwort mit Passwortmanager ändern"
date: "2014-05-22"
categories: 
  - "tech"
tags: 
  - "ebay"
  - "password"
---

**English version below.**

Zurzeit ist ebay in den Nachrichten, da sie Zugriffe auf Passwörter der Nutzer festgestellt haben.

Leider haben sie merkwürdige Sicherheitsregeln beim Ändern des Passworts. Sie unterbinden die Verwendung von Copy/Paste. Was zur Folge hat, dass man keinen Passwortmanager verwenden kann.

Falls man dennoch einen Passwortmanager verwenden will, muss man wie folgt vorgehen.

 

Man öffnet die Konsole des Browsers (Firefox-Mac Command + Alt + K). Dort gibt man nun folgendes ein:

>  document.getElementById("password").value = "password";

und

> document.getElementById("retypepassword").value = "password";

password muss man durch sein persönliches Passwort ersetzen. Nun erscheinen die Passwörter in Form von kleinen Punkten in den Feldern.

**English Version**

At the moment ebay is in the news for getting hacked.

Unfortunately when changing your password ebay prevents you from using copy/paste thus preventing password managers.

To bypass this issue you have to use the console of your browser (Firefox-Mac Command + Alt + K). Follow these steps:

>  document.getElementById("password").value = "password";

and

> document.getElementById("retypepassword").value = "password";

In these commands you have to change password to your new password. If it worked you will see the typical dots in the password fields.
