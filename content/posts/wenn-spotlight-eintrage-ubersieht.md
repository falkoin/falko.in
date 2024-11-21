---
title: "Wenn Spotlight Einträge übersieht"
date: "2015-12-02"
---

Vor ein paar Tagen konnte ich MATLAB nicht mehr über Spotlight starten, was ich in der Regel mehrmals pro Woche tue.

Mit einem erneuten Laden der Metadaten kann man das Problem beheben:

> ```
> sudo mdutil -a -i off
> ```

Deaktivieren von Spotlight

> ```
> sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.metadata.mds.plist
> ```

Verweis auf Metadaten entfernen

> ```
> sudo launchctl load -w /System/Library/LaunchDaemons/com.apple.metadata.mds.plist
> ```

Verweis wieder erstellen

> ```
> sudo mdutil -a -i on
> ```

Aktiveren von Spotlight

 

Die Lösung stammt nicht von mir, sondern kommt von [hier](https://apple.stackexchange.com/questions/62715/applications-dont-show-up-in-spotlight).
