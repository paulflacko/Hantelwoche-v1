# Werkzeuge für die Bilder

## Fotos (`img/foto/*.webp`)
Quelle: [free-exercise-db](https://github.com/yuhonas/free-exercise-db) (Unlicense, gemeinfrei).
Je Übung zwei Fotos (Start und Ende), verkleinert auf 480 × 320 und als WebP-Animation mit Markierung 1/2 gespeichert.

1. Fotos laden: `https://raw.githubusercontent.com/yuhonas/free-exercise-db/main/exercises/<ID>/0.jpg` und `1.jpg` nach `<ordner>/<ID>/`
2. Zuordnung pflegen: `fotos/map_existing.py` (bestehende Übungen) und `fotos/new_ex.py` (neue Übungen mit deutschen Texten)
3. Bauen: `python3 fotos/mkphotos.py <ordner> ../img/foto`

Die Zuordnung steht in der App als `PH` (Schlüssel → Datei, optional Hinweis, wenn das Foto ein anderes Gerät zeigt).

## Eigene Animationen (`img/yoga-*.gif` u. a.)
Eigene Strichfiguren mit Vorwärtskinematik, gerendert mit Pillow (`animationen/fig.py`). Frei nutzbar (CC0).
- `poses.py` Posen, `mobility2.py` rendert alle Mobility/Yoga-Animationen mit leuchtendem Zielbereich nach `out2/`
- `yoga2.py` neue Haltungen (Kobra, Baum, Dreieck, Stuhl, Girlande, Schmetterling, Vorbeuge sitzend) nach `out3/`
- `einstieg.py` Unterarmstütz und Aufwärmsätze nach `out/`
- `ZOOM` in `fig.py` steuert, wie stark die Figur das Bild füllt (seit 2026-11: 1,6 statt 1,0, dadurch deutlich größer)
