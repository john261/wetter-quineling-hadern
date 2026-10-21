# Wetter-Quineling – GitHub Pages

Öffentliche, mobile Wetterübersicht für München-Hadern. Beim Aufruf fragt die Browserseite die kostenlose Open-Meteo Forecast API ab; bei geöffneter Seite wird alle zehn Minuten aktualisiert. Die Seite benötigt weder API-Key noch Backend.

## Auf GitHub veröffentlichen

1. Ein öffentliches GitHub-Repository anlegen.
2. Den Inhalt dieses Ordners in das Stammverzeichnis des Repositorys hochladen (also `index.html` direkt im Repository-Root).
3. In GitHub unter **Settings → Pages** als Quelle **Deploy from a branch**, Branch `main` und Ordner `/ (root)` auswählen.
4. Nach der Veröffentlichung die von GitHub angezeigte Pages-Adresse auf Handy und anderen Geräten öffnen.

Die Website ist öffentlich. GitHub Pages führt kein Python im Hintergrund aus; die Wetterdaten werden nur beim Öffnen, beim manuellen Aktualisieren und während die Seite sichtbar geöffnet ist, abgerufen. Desktop-Benachrichtigungen des lokalen Quineling bleiben eine separate Funktion des Python-Programms.

## Daten und Regeln

- Fest eingestellt auf München-Hadern (48.1147, 11.4822), Europe/Berlin.
- Regen nach Regel: Niederschlagswahrscheinlichkeit mindestens 50 % **oder** Niederschlag mindestens 0,1 mm.
- API-Ausfälle zeigen den letzten erfolgreichen Tagesabruf aus demselben Browser, wenn verfügbar.
- Quelle: [Open-Meteo](https://open-meteo.com/).
