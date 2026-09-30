# Recherche: Was kostet ein eigener KI-Assistent für Firmenwissen?
Stand: 25.09.2026

| # | Behauptung | Beleg (eigene Worte) | Quelle | Datum | Sicherheit |
|---|---|---|---|---|---|
| F1 | Azure OpenAI rechnet im Standardmodell nach verbrauchten Tokens ab, getrennt für Eingabe und Ausgabe | Microsoft beschreibt „Standard" als nutzungsbasierte Abrechnung pro Eingabe- und Ausgabe-Token | [Azure OpenAI – Preise](https://azure.microsoft.com/de-de/pricing/details/cognitive-services/openai-service/) | Seite aktualisiert 09/2026 | hoch |
| F2 | Alternativ gibt es reservierte Kapazität (Provisioned Throughput) mit planbaren Kosten | Monatliche und jährliche Reservierungen verfügbar | wie F1 | 09/2026 | hoch |
| F3 | Bei „Data Zone Standard" (EU) werden Daten innerhalb der EU-Datengrenze verarbeitet, gespeicherte Daten bleiben in der gewählten Azure-Geografie | Microsoft-Doku zu Bereitstellungstypen | [Deployment types – Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-foundry/foundry-models/concepts/deployment-types) | 12.08.2026 | hoch |
| F4 | Azure AI Search im Modell „Dedicated" wird pro Stunde abgerechnet (Sucheinheiten × Stundenpreis), nicht pro Suchanfrage | Kosten = Replikate × Partitionen × Stundenpreis der Stufe; keine Abrechnung pro Anfrage | [Plan and manage costs – Azure AI Search](https://learn.microsoft.com/en-us/azure/search/search-sku-manage-costs) | 02.07.2026 | hoch |
| F5 | Dedicated-Suchdienste kosten auch ohne Nutzung weiter, nur Löschen stoppt die Abrechnung | wie F4 | wie F4 | 02.07.2026 | hoch |
| F6 | Es gibt ein Serverless-Modell (Vorschau) ohne Rechenkosten im Leerlauf, nur Speicher wird berechnet | wie F4 | wie F4 | 02.07.2026 | mittel (Vorschau) |

## Aus kontext/ (Insight AI)
| # | Aussage | Datei |
|---|---|---|
| K1 | Aufbau KI-Infrastruktur 4.000–10.000 € einmalig | kontext/unternehmen.md |
| K2 | Daten-Pipeline je Quelle 5.000–8.000 € einmalig | kontext/unternehmen.md |
| K3 | Betrieb und Weiterentwicklung ab 2.000 €/Monat, Partnerschaft lässt sich herunterfahren | kontext/unternehmen.md |
| K4 | Typisches Erstprojekt 15.000–25.000 € einmalig | kontext/unternehmen.md |
| K5 | KI-Anwendung: Kunde baut selbst mit Copilot Studio oder separat kalkuliert | kontext/unternehmen.md |
| K6 | Infrastruktur umfasst Modell-Endpunkte, Wissensbasis (Vektorisierung), RBAC, abgesicherte Speicher | kontext/unternehmen.md |
| K7 | Pipeline: Anbindung, Bereinigung, Segmentierung, Metadaten, optional Entfernung personenbezogener Daten, tägliche Synchronisation | kontext/unternehmen.md |
| K8 | Azure-Verbrauch läuft direkt zwischen Kunde und Microsoft, ein Vertrag, eine Rechnung | kontext/unternehmen.md |
| K9 | enGPT (Softengine): 15.000+ Dokumente, täglich aktualisiert, 1,5 Jahre produktiv | kontext/freigaben.md |
| K10 | Alle Preise zzgl. USt. | kontext/unternehmen.md |
| K11 | Entwicklung in Azure- und GitHub-Umgebung des Kunden, Code, Infrastruktur und Doku bleiben beim Kunden | kontext/unternehmen.md |

<!-- K11 nachgetragen in Faktencheck-Runde 1 (siehe 06-faktencheck.md) -->

## Nicht belegbar
- Konkrete Euro-Beträge für den monatlichen Azure-Verbrauch → nicht nennen, bis Thomas Erfahrungswerte liefert
- Vergleich mit Lizenzkosten für Microsoft 365 Copilot → Preise haben sich 2026 mehrfach geändert, eigenes Thema (T2)

## Offen für Thomas
- Größenordnung der monatlichen Azure-Kosten in bisherigen Projekten
- Häufigster unterschätzter Kostenfaktor
- Interner Zeitaufwand beim Kunden
