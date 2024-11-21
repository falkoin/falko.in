---
title: "OS X Videos richtig convertieren"
date: "2013-02-10"
categories: 
  - "tech"
tags: 
  - "ffmpeg"
  - "video"
  - "video-convertion"
---

Ich musste mich mal wieder mit dem leidigen Thema "Videokonvertierung" beschäftigen. Ziel war es ein Video (.MTS) am Mac zu bearbeiten und anschließend Windows Power Point tauglich (.MPG) zu machen. Wenn man ganz normal in einer Suchmaschine nach den Begriffen "Video", "Konvertierung" und "Mac" sucht, bekommt man fast ausschließlich kostenpflichtigen Schrott unter die Nase gerieben. Mit [FFmpeg](http://www.ffmpeg.org/) bin ich fündig geworden. Dabei handelt es sich um ein mächtiges Kommandozeilen-Tool. Ist zunächst nicht ganz einfach, einmal durchblickt aber unheimlich komfortabel. Daher im folgenden eine kleine Anleitung:

**FFmpeg** installieren (am besten mit MacPorts).

> sudo port install ffmpeg

Anschließend einfach

> ffmpeg -i videoname.in -qscale 0 videoname.out

und fertig ist das neue Video. Dabei ist zu beachten, dass die Output-Endung das Format bestimmt. Unterstützte Formate kann man sich mit

> ffmpeg -formats

ansehen. Der Parameter "-qscale 0" bewirkt, dass mit quasi gleicher Qualität konvertiert wird.

Umwandeln von .MOV zu .MPEG hat bei mir problemlos funktioniert.
