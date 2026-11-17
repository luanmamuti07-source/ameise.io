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
- **Schlecht:** Jagdspinne, Ameisenlöwe, Riesenschuh, Regenschauer, Marienkäfer (fressen Blattläuse)

### Blattlaus-Weiden

Im Bau-Menü legst du bis zu zwei Weiden pro Bau an (max. 900 vom Bau entfernt, 150 Futter). Die Läuse vermehren sich langsam und liefern dauerhaft Honigtau, der sich in der Weide sammelt (max. 500), bis deine Sammlerinnen ihn abholen. Weiden lassen sich bis Stufe 3 ausbauen.

Das Risiko: Wer eine Weide überfällt, bekommt den gelagerten Honigtau. Zerstört eine Legion die Weide, stiehlt sie außerdem die Hälfte der Läuse. Marienkäfer-Schwärme fressen Läuse, wenn keine Kämpferinnen in der Nähe sind.

### Königinnen-Raub

Zerstört eine Legion einen fremden Bau, nimmt sie die Königin gefangen. Bringt sie sie lebend in einen eigenen Bau, gibt es Ameisen, Futter, gestohlene Fähigkeiten und Bernstein, gegen die Nummer 1 der Bestenliste doppelt. Die Gefangene ist langsam, und alle in der Nähe versuchen, sie zu befreien.

### Weitere Systeme

- **Nebel des Krieges:** Du siehst nur, was deine Ameisen sehen. Auch die Bots kennen nur, was sie erkundet haben.
- **Legionen zusammenstellen:** Du bestimmst, wie viele Kämpferinnen jeder Art mitgehen, und steuerst mehrere Legionen gleichzeitig.
- **Reichsübersicht:** Alle Baue mit Truppen, Futter und Weiden auf einen Blick.
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
| O | Reichsübersicht |
| R | Legion zusammenstellen (Shift + R: alle Kämpferinnen) |
| 1–5 | Legion wählen, dann auf die Karte klicken (fremder Bau = Überfall) |
| Shift + 1–5 / Shift + Klick | Mehrere Legionen wählen |
| Q | Alle Legionen wählen |
| H / X | Legion heim schicken / auflösen |
| B | Nächsten eigenen Bau öffnen |
| Leertaste | Kamera auf Legion oder Bau zentrieren |
| Esc | Fenster schließen, Auswahl aufheben |

## Technik

Reines HTML, CSS und JavaScript mit Canvas-Grafik, ohne Bibliotheken. Nur die Schriftarten kommen von Google Fonts.
