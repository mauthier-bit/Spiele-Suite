# Spiele-Suite – Mathematik & Physik

Zwölf Unterrichtsspiele für das iPad, zusammengefasst auf einer Startseite.
Alle Spiele sind **einzelne HTML-Dateien ohne externe Abhängigkeiten**: kein Server,
keine Anmeldung, keine Internetverbindung nötig. Einmal geladen, laufen sie offline.

**Start:** [`index.html`](index.html)

## Die Spiele

| Spiel | Jahrgang | Thema | Spielform |
|---|---|---|---|
| [Memory](memory.html) | 5 – 13 | 73 Kartensätze: Darstellungen verknüpfen | Paare aufdecken, 1 – 4 Spieler |
| [Bruno](Bruno.html) | 6 (ab 7 zur Wiederholung) | Brüche und ihre Darstellungen | Kartenspiel, zu zweit oder gegen den Computer |
| [D-Uno](D-Uno.html) | 5 – 7 | Distributivgesetz, Aus­klammern und Aus­multiplizieren | Kartenspiel, zu zweit oder gegen den Computer |
| [Termino](Termino.html) | 7 – 10 | gleichwertige Terme | Domino, gegeneinander oder kooperativ |
| [Fumino](Fumino.html) | 8 – 10 | Funktionsterm und Graph zuordnen | Domino, gegeneinander oder kooperativ |
| [Kopfrechen-Duell](Kopfrechen-Duell.html) | 5 – 11 | Kopfrechnen und Grundwissen auf Zeit | Team-Duell für die ganze Klasse |
| [Mattle](Mattle.html) | 5 – 11 | Kopfrechnen mit Strategie (Hex-Spielfeld) | Team-Duell für die ganze Klasse |
| [Galgenmännchen](galgenmaennchen.html) | 5 – 13 | 475 Fachbegriffe aus dem LehrplanPLUS erraten | ganze Klasse, allein oder zwei Teams |
| [Mathe-Tabu](mathe-tabu.html) | 5 – 13 | Fachbegriffe versprachlichen | Erklärspiel, zwei Teams |
| [Physik-Tabu](physik-tabu.html) | 7 – 13 | physikalische Fachbegriffe versprachlichen | Erklärspiel, zwei Teams |
| [Schiffe versenken](schiffe-versenken-koordinaten.html) | 5 | Koordinaten setzen und ablesen | Duell zu zweit oder gegen den Computer |
| [Raumschiffe versenken](raumschiffe-versenken.html) | Oberstufe | räumliches Koordinatensystem, Punkte und Vektoren | Duell zu zweit oder gegen den Computer |

Die Startseite beschreibt jedes Spiel ausführlich und lässt sich nach Fach,
Jahrgangsstufe und Spielform filtern.

## Teilen per QR-Code

Jedes Spiel hat auf seinem Startbildschirm einen **Teilen**-Knopf. Er zeigt einen großen
QR-Code, den die Schülerinnen und Schüler mit der Tablet-Kamera scannen – das Spiel öffnet
sich dann direkt auf ihrem Gerät. Der Code wird offline erzeugt, ohne Internetdienst.

Wird die Seite über GitHub Pages aufgerufen, zeigt der Code auf genau diese Adresse. Beim
Öffnen einer lokalen Datei nimmt er stattdessen die veröffentlichte Fassung unter
`https://mauthier-bit.github.io/Spiele-Suite/`; über „Adresse ändern“ lässt sich das im
Spiel anpassen (die Angabe wird im Browser gespeichert).

## Benutzen

**Lokal:** Ordner herunterladen, `index.html` im Browser öffnen. Alle Spiele
liegen flach daneben und werden relativ verlinkt – der Ordner muss zusammenbleiben.

**GitHub Pages:** Repository anlegen, den Inhalt dieses Ordners hochladen und unter
*Settings → Pages* die Quelle auf den Branch (Ordner `/root`) stellen. Die Suite ist
dann direkt unter der Pages-Adresse erreichbar, weil die Startseite `index.html` heißt.
Die leere Datei `.nojekyll` sorgt dafür, dass GitHub die Dateien unverändert ausliefert.

**Auf dem iPad:** Seite in Safari öffnen und über *Teilen → Zum Home-Bildschirm*
ablegen – die Suite startet dann wie eine App im Vollbild.

## Ein Spiel ergänzen

Neue HTML-Datei in den Ordner legen und in `index.html` im Array `GAMES`
ein Objekt ergänzen (Dateiname, Titel, Kurztext, Jahrgangsstufen, Spielform,
Stichwörter für die Suche). Sonst ist nichts zu ändern.

> Die Dateinamen werden **genau so** verlinkt, wie sie heißen. Auf GitHub Pages
> wird Groß- und Kleinschreibung unterschieden – beim Umbenennen also auch die
> Einträge in `index.html` anpassen.
