---
name: rezept-format
description: Format für alle Rezepte in jojo-kocht. Verwenden, wenn ein neues Rezept angelegt oder ein bestehendes Rezept umformatiert wird. Ziel ist "easy to read": Einleitung, eine komplette Zutatenliste, eine Zubereitungstabelle Zeit | Zutaten | Aktion, Profi-Tipp.
---

# Rezept-Format

Ziel: Das Rezept muss sich beim Kochen auf einen Blick lesen lassen. Kurz, klar, keine langen Absätze in der Zubereitung.

## Aufbau (immer in dieser Reihenfolge)

1. `# Titel` (eine H1 pro Datei)
2. `*Bearbeitet: <Datum>*` nur wenn bekannt, nie erfinden
3. `*Einleitung.*` kursiv, 2 bis 4 Sätze: was es ist, was es besonders macht, wichtige Varianten (z. B. andere Hefemenge bei kürzerer Gare)
4. `*Portionen: ... Aktive Zeit ..., Gare ..., Backzeit ...*` kursiv, eine Zeile
5. `## Zutaten`: **eine** komplette Liste mit `-`, alle Zutaten mit Menge, auch die zum Bestreichen oder Belegen. Keine Unterüberschriften, keine Tabelle.
6. `## Zubereitung`: **eine** Tabelle mit den Spalten `Zeit | Zutaten | Aktion`
7. `## Profi-Tipp`: ein kurzer Absatz mit den wichtigsten Tricks und Fehlerquellen

## Regeln für die Zubereitungstabelle

- **Zeit:** konkrete Uhrzeit (`14:00`) aus einem Beispiel-Zeitplan, sonst relative Angabe (`danach`, `+1 Std.`). Bei Rezepten über mehrere Tage den Tag dazuschreiben (`Fr 16:00`).
- **Zutaten:** nur was in diesem Schritt dazukommt, jede Zutat mit Menge, mehrere mit `<br>` untereinander. Zwischenprodukte beim Namen nennen (`Hefemilch`, `Teig`, `Kugeln`). Geräte wie `Plancha` oder `Ofen` dürfen hier stehen, wenn der Schritt nur das Gerät betrifft.
- **Aktion:** wenige Wörter, klein geschrieben, Kommas statt ganzer Sätze. Zeiten und Temperaturen rein, Erklärungen raus (die gehören in Einleitung oder Profi-Tipp).
- Ein Schritt pro Zeile, maximal ca. 10 Zeilen.

## Allgemeine Regeln

- Sprache Deutsch, Mengen in g / ml / Stück, `°C`, `Min.`, `Std.`
- Keine `*`-Aufzählungen, keine `---`-Linien, keine Blockquotes, kein Frontmatter
- Keine Gedankenstriche (—)
- Dateiname klein, mit Bindestrichen (`naan-plancha.md`), Rezept in `README.md` unter Rezepte verlinken
- Beim Umformatieren eines bestehenden Rezepts Mengen nie ändern
- Nach dem Commit immer pushen

## Beispiel

```markdown
# Schnelles Naan auf der Plancha

*Weiches, blasiges Naan mit Hefe und Joghurt, ohne Kaltgare. Der Teig geht ca. 2,5 Std. warm und wird dann direkt auf der heißen Plancha gebacken. Bei nur 1 Std. Gare 15 g statt 10 g frische Hefe nehmen.*

*Portionen: 8 Naan (je ca. 120 g). Aktive Zeit ca. 30 Min., Gare ca. 2,5 Std., Backzeit ca. 2 Min. pro Stück.*

## Zutaten

- 500 g Weizenmehl Type 550
- 250 g Joghurt, 3,5 % Fett, zimmerwarm
- 140 ml lauwarme Milch
- 10 g frische Hefe
- 10 g Zucker
- 10 g Salz
- 30 ml neutrales Öl
- 40 g Butter oder Ghee
- 1 Knoblauchzehe

## Zubereitung

| Zeit | Zutaten | Aktion |
| --- | --- | --- |
| 14:00 | 140 ml lauwarme Milch<br>10 g frische Hefe<br>10 g Zucker | verrühren, 5 Min. stehen lassen |
| 14:05 | 500 g Mehl 550<br>250 g Joghurt 3,5 %<br>10 g Salz<br>30 ml Öl<br>Hefemilch | 10 Min. kneten, abgedeckt warm gehen lassen |
| 16:35 | Teig | in 8 Kugeln teilen, 10 Min. ruhen lassen |
| 16:45 | Plancha | ohne Öl auf mittlere bis hohe Hitze vorheizen |
| 17:00 | Kugeln | dünn ausrollen, je ca. 1 Min. pro Seite braten |
| danach | 40 g geschmolzene Butter<br>1 Knoblauchzehe, gerieben | heiße Naan bestreichen, im Tuch warm halten |

## Profi-Tipp

Die Plancha nicht einölen, Naan wird trocken gebacken, sonst frittiert es und wird nicht blasig. Wird der Fladen zu dunkel, bevor er Blasen wirft, die Hitze etwas senken.
```

Vorlage im Repo: `naan-plancha.md`
