---
name: themen
description: Füllt den Themenpool von Insight AI mit neuen, bewerteten Artikelideen aus echten Fragen der Zielgruppe.
disable-model-invocation: true
argument-hint: "[Anzahl, Standard 5] [optionaler Schwerpunkt]"
---

# /themen

Auftrag: **$ARGUMENTS** (ohne Angabe 5 Themen, ohne Schwerpunkt über alle Leistungen verteilt)

1. Starte **themen-scout** im Modus 2 mit Anzahl und Schwerpunkt.
2. Prüfe, dass jede neue Zeile in `themen/themenpool.md` eine eindeutige ID (T…), alle vier Bewertungen und Status `idee` hat.
3. Gib die drei Themen mit der höchsten Summe aus und schlage vor, mit welchem `/artikel` gestartet werden soll.
