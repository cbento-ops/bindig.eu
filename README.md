# bindig.eu

Quelltext der persönlichen Website von Christopher Bindig: <https://bindig.eu>

Statisches HTML mit einem Stylesheet. Kein Build-Schritt, keine Abhängigkeiten, keine Cookies, kein Tracking, keine externen Schriften.

## Aufbau

| Datei | Zweck |
|---|---|
| `index.html` | Startseite, Deutsch |
| `en/index.html` | Startseite, Englisch |
| `style.css` | Gestaltung für alle Seiten |
| `portrait.jpg` | Porträt |
| `404.html` | Fehlerseite |
| `robots.txt`, `sitemap.xml` | Angaben für Suchmaschinen |
| `CNAME` | verbindet das Repository mit der Domain bindig.eu |
| `.nojekyll` | GitHub Pages liefert die Dateien unverändert aus |

## Lokal ansehen

Die Seiten binden Stylesheet und Bild mit Pfaden ab der Wurzel ein (`/style.css`). Per Doppelklick geöffnet erscheinen sie deshalb ohne Gestaltung. Zum Ansehen einen lokalen Webserver im Ordner dieses Repositorys starten:

```sh
python3 -m http.server 8080
```

Danach <http://localhost:8080> im Browser öffnen. Der Server läuft nur auf dem eigenen Rechner und nur, solange der Befehl läuft; beenden mit `Ctrl + C`.

## Veröffentlichen

Jeder Push auf `main` wird von GitHub Pages nach etwa einer Minute unter <https://bindig.eu> ausgeliefert.
