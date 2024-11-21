---
title: "Spyder sehr langsam unter macOS Mojave"
date: "2019-08-02"
---

Ich arbeite in letzter Zeit viel mit Python, bevorzugt in der IDE Spyder. Leider ist diese irgendwann ziemlich langsam geworden.

Wie [dieser GitHub Issue Tracker](https://github.com/spyder-ide/spyder/issues/2902) verdeutlicht, bin ich nicht der einzige mit diesem Problem.

Abhilfe hat bei mir die [Antwort von **ccordoba12**](https://github.com/spyder-ide/spyder/issues/2902#issuecomment-483170998) geschaffen:

> conda install ipython=6 ipykernel=4

Das Ausführen im Terminal hat ziemlich lange gedauert, aber danach läuft Spyder wieder schön rund.
