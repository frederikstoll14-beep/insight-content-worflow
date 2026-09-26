---
name: linkedin
description: Macht aus einem freigegebenen Artikel-Laufordner drei geprüfte LinkedIn-Beiträge für Thomas Weller inklusive Timing und Verteilung.
disable-model-invocation: true
argument-hint: <Laufordner, z. B. content/2026-09-25-kosten-ki-assistent>
arguments: [ordner]
---

# /linkedin

Laufordner: **$ordner**

1. Prüfe, dass `$ordner/05-artikel.md` und `$ordner/06-faktencheck.md` existieren und der Faktencheck FREIGABEFÄHIG ist. Sonst abbrechen und sagen, was fehlt.
2. Starte **linkedin-redakteur** mit dem Laufordner.
3. Starte **stil-pruefer** für `$ordner/linkedin.md` im Profil `linkedin`.
4. Enthält `linkedin.md` einen Karussell-Abschnitt, starte **visual-designer** für die Folien (1080×1350).
5. Gib die drei Beiträge vollständig aus, darunter je Tag, Uhrzeit und Zielgruppe. Keine automatische Veröffentlichung.
6. Trage die geplanten Beiträge als leere Zeilen in `auswertung/metriken.csv` ein (Kennzahlen füllt der Mensch nach 7 Tagen).
