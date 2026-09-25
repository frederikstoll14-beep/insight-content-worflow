# Faktencheck

## Runde 1
Ergebnis: **NACHARBEIT NÖTIG**

| Stelle (Zitat) | ID | Befund | Empfehlung |
|---|---|---|---|
| „Die Wahl des Sprachmodells ist dagegen meist ein kleinerer Faktor." | – | ohne Beleg | Streichen oder als Erfahrungswert von Thomas mit `[OFFEN]` belegen |
| „Gehören Code und Daten mir? Ja, alles liegt in Ihrer eigenen Azure- und GitHub-Umgebung." | – | ohne Beleg (inhaltlich in kontext/unternehmen.md vorhanden, aber keine ID) | ID in 02-recherche.md ergänzen (K11) |
| „Dann rechnen sich die festen Kosten der Suche kaum." | F5 | Verschärfung: F5 sagt nur, dass Kosten ohne Nutzung weiterlaufen, nicht, ob es sich rechnet | Als Begründung formulieren, keine Wirtschaftlichkeitsaussage |
| Rechenbeispiel ohne Hinweis auf Annahmen | K1, K2 | Einzelwerte sind Annahmen, nicht veröffentlichte Preise | Kennzeichnen als Annahme innerhalb der Spannen |
| „Preise" ohne Umsatzsteuerhinweis | K10 | unvollständig | „zzgl. USt." ergänzen |

## Runde 2
Ergebnis: **FREIGABEFÄHIG**

| Stelle (Zitat) | ID | Befund |
|---|---|---|
| „kostet 15.000 bis 25.000 € einmalig" | K4 | korrekt |
| „Betreuung ab 2.000 €" · „lässt sich herunterfahren" | K3 | korrekt |
| „Sobald Sie mehr als eine Datenquelle anbinden, entfällt der größere Teil der Einmalkosten auf die Daten" | K1, K2 | korrekt: ab zwei Quellen mindestens 10.000 € Pipelines gegenüber höchstens 10.000 € Infrastruktur. Grenzfall bei exakt 2 × 5.000 € und 10.000 € Infrastruktur (Gleichstand), vertretbar |
| „Alle Preise in diesem Artikel verstehen sich zuzüglich Umsatzsteuer." (Rechenbeispiel) | K10 | korrekt |
| Infrastruktur-Bestandteile, 4.000 bis 10.000 € | K6, K1 | korrekt |
| Pipeline-Schritte, 5.000 bis 8.000 € pro Quelle | K7, K2 | korrekt |
| Oberfläche mit Copilot Studio ohne Projektkosten | K5 | korrekt („Ihr Team entwickelt selbst … Wir liefern Infrastruktur und Wissensbasis") |
| Abrechnung pro Token, getrennt nach Ein- und Ausgabe | F1 | korrekt, Quelle erneut geöffnet |
| Reservierte Kapazität monatlich oder jährlich | F2 | korrekt |
| Suche pro Stunde, unabhängig von Anfragen | F4 | korrekt, Quelle erneut geöffnet |
| Nur Löschen beendet die Abrechnung | F5 | korrekt |
| Serverless-Modell in Vorschau, im Leerlauf nur Speicher | F6 | korrekt, Vorschau-Status genannt |
| Rechenbeispiel als Annahme gekennzeichnet | K1, K2, K4 | korrekt, 8.000 + 6.000 + 7.000 = 21.000 nachgerechnet |
| Data Zone Standard EU | F3 | korrekt. Hinweis: Quelle spricht von „Azure-Geografie", Artikel sagt „Azure-Region". Vertretbar für Zielgruppe, bei Bedarf präzisieren |
| enGPT, 15.000+ Dokumente, 1,5 Jahre | K9 | korrekt, Status „frei" in freigaben.md |
| Code, Infrastruktur, Doku beim Kunden | K11 | korrekt |

## Offene Punkte für Thomas
- 3 × `[OFFEN]` im Text (Azure-Monatskosten, unterschätzter Faktor, Veränderung bei Softengine). Der Artikel ist ohne sie veröffentlichbar, wird mit ihnen aber deutlich stärker.
- Freigabe, dass enGPT in diesem Kontext (Kostenartikel) genannt werden darf.
