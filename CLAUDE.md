# Spiele-Suite

Veröffentlichungs-Ordner der Unterrichtsspiele, live unter
https://mauthier-bit.github.io/Spiele-Suite/ (Repo `mauthier-bit/Spiele-Suite`, öffentlich).
Allgemeine Regeln stehen in `~/git/CLAUDE.md`.

## Wo geändert wird

- **Master ist nicht dieser Ordner**, sondern `~/Documents/Schule/Temp Schule/FB/Spiele/`.
  Dort ändern, dann mit `~/git/sync-spiele.sh` verteilen (`--probe` zeigt vorher, was passiert,
  `--commit` committet beide Repos und pusht diese Suite).
- Hier heißt die Übersicht `index.html`, im Master und in `~/git` `Spiele-Suite.html`.
- Neues Spiel: Datei in den Master, Dateinamen ins Array `SPIELE` in `sync-spiele.sh` und
  ein Objekt ins Array `GAMES` der Übersicht.

## Aufbau der Übersicht

- Filter nach Fach, Jahrgang (5–6/7–8/9–10/11–13), Spielform (Array `FORMEN`) und Volltextsuche
  über `keywords`; Karten mit Detail-Fenster je Spiel.
- Ein `GAMES`-Eintrag: `file, title, tagline, icon, color, fach, form, stufen` (Zahlen, steuern den
  Jahrgangsfilter), `stufenText, sozial, thema, kurz, ziel, punkte[], keywords`.
- Links sind relativ und groß-/kleinschreibungsempfindlich. Beim Umbenennen `GAMES` nachziehen.

## In jedem Spiel

- Teilen-Knopf mit QR-Code (siehe `~/git/CLAUDE.md`). Er erscheint nur auf dem Startbildschirm
  (`var ANCHOR`) oder sitzt in einer Leiste (`var INLINE`), je nach Spiel.
- Streifen gegen den iPadOS-Statusleisten-Verlauf. Er übernimmt die Hintergrundfarbe vom `body`,
  ein reiner Verlauf als Hintergrund braucht deshalb zusätzlich `background-color`.
- `kantentest.html` ist eine Testseite für diesen Streifen, kein Spiel.
