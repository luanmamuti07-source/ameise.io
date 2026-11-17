# Ameisenreich

**Ein Ameisen-Strategiespiel für den Browser.** Gründe eine Kolonie, baue deinen Bau aus, entwickle sechs Ameisenarten und führe Legionen gegen 18 andere Kolonien in die Schlacht.

Das ganze Spiel steckt in einer einzigen Datei (`ameisenreich.html`). Es braucht keine Installation und keinen Server: Datei herunterladen, im Browser öffnen, spielen.

## Spielen

- **Lokal:** `ameisenreich.html` herunterladen und doppelklicken.
- **Online über GitHub Pages:** In den Repo-Einstellungen unter *Settings → Pages* als Quelle den Branch `main` und den Ordner `/ (root)` wählen. Danach läuft das Spiel unter `https://luanmamuti07-source.github.io/ameise.io/`.

## Worum es geht

Deine Königin lebt in einem Bau. Sammlerinnen holen Futter, damit baust du Räume aus und brütest neue Ameisen. Mit Kämpferinnen verteidigst du deine Baue, überfällst fremde Kolonien und raubst ihr Futter. Wenn ein Bau groß genug ist, schickst du eine junge Königin los und gründest einen weiteren Bau.

### Baue und Räume

| Raum | Wirkung |
| --- | --- |
| Königinnenkammer | Stufe des Baus: mehr Leben, Plätze, Revier und Raum-Stufen |
| Brutkammer | Königin legt schneller Eier |
| Vorratskammer | Mehr Lager und Sammler-Plätze |
| Kriegerquartier | Mehr Armee-Plätze |
| Kaserne | Stärkere Kämpferinnen, billigere Eier |
| Pilzgarten | Futter wächst von selbst |
| Wachkammer | Der Bau spuckt Säure auf Angreifer |

Jeder Bau hat **eigenes Futter** und **getrennte Plätze** für Sammlerinnen und Armee. Im Logistik-Fenster verschiebst du Futter und Ameisen zwischen deinen Bauen.

### Ameisenarten

| Art | Rolle | Freigeschaltet durch |
| --- | --- | --- |
| Sammlerin | Sammelt Futter in Revier und markierten Sammelgebieten | von Anfang an |
| Trägerin | Nimmt Sammlerinnen das Futter ab und schleppt es heim | 4 Punkte im Sammlerinnen-Baum |
| Kriegerin | Nahkampf | von Anfang an |
| Spuckerin | Säure auf Distanz | 3 Punkte im Kriegerinnen-Baum |
| Riesin | Riesig, zäh, trifft mehrere Gegner | 7 Punkte im Kriegerinnen-Baum |
| Sprengameise | Rennt in den Feind und explodiert | 5 Punkte im Spuckerinnen-Baum |

Jede Art hat ihren eigenen **Fähigkeitsbaum**. Kämpferinnen bekommen zusätzlich **einmalige Spezialisierungen**, bei denen du aus 3–4 Möglichkeiten eine wählst, zum Beispiel Berserkerin, Giftbiss, Scharfschützin, Rammbock oder Tarnung.

### Ereignisse

Etwa alle 30–50 Sekunden passiert etwas in der Welt:

- **Gut:** Riesenkäfer (900 Futter als Beute), Regenwürmer, heruntergefallenes Eis, Picknick-Krümel
- **Schlecht:** Jagdspinne, Ameisenlöwe, Riesenschuh, Regenschauer

### Weitere Systeme

- **Nebel des Krieges:** Du siehst nur, was deine Ameisen sehen.
- **Ausbildungs-Warteschlange:** Einheiten gezielt in Auftrag geben. Ist die Schlange leer, schlüpfen automatisch Sammlerinnen.
- **Bernstein und Skins:** Nach jeder Runde und täglich gibt es Bernstein für dauerhafte Startboni und Ameisen- oder Bau-Skins. Er wird im Browser gespeichert.

## Steuerung

| Eingabe | Aktion |
| --- | --- |
| Ziehen / WASD / Pfeiltasten | Karte bewegen |
| Mausrad / Pinch | Zoom |
| Klick auf eigenen Bau | Bau-Menü |
| E | Evolution |
| L | Logistik |
| R | Legion aus der Garnison ausheben |
| 1–5 | Legion wählen, dann auf die Karte klicken (fremder Bau = Überfall) |
| H / X | Legion heim schicken / auflösen |
| B | Nächsten eigenen Bau öffnen |
| Leertaste | Kamera auf Legion oder Bau zentrieren |
| Esc | Fenster schließen, Auswahl aufheben |

## Technik

Reines HTML, CSS und JavaScript mit Canvas-Grafik, ohne Bibliotheken. Nur die Schriftarten kommen von Google Fonts.
