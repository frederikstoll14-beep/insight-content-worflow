---
titel: Was kostet ein eigener KI-Assistent für Firmenwissen?
meta_beschreibung: Was ein KI-Assistent für Firmenwissen im Mittelstand kostet, einmalig und monatlich, und wovon der Preis abhängt. Mit Rechenbeispiel.
hauptfrage: Was kostet ein eigener KI-Assistent für unser Firmenwissen?
nebenfragen:
  - "Welche Kosten fallen einmalig an?"
  - "Was kostet das Sprachmodell?"
  - "Gibt es Kosten ohne Nutzung?"
  - "Wovon hängt der Preis ab?"
  - "Kann man klein anfangen?"
zielgruppe: Geschäftsführung
stand: 2026-09-25
---

# Was kostet ein eigener KI-Assistent für Firmenwissen?

Ein typisches erstes Projekt für einen KI-Assistenten, der auf Ihr Firmenwissen zugreift, kostet 15.000 bis 25.000 € einmalig. <!-- K4 --> Dazu kommen monatlich die nutzungsabhängigen Kosten bei Microsoft Azure und, wenn Sie das möchten, eine Betreuung ab 2.000 €. <!-- K3 --> Sobald Sie mehr als eine Datenquelle anbinden, entfällt der größere Teil der Einmalkosten auf die Daten und nicht auf die KI-Infrastruktur. <!-- K1 K2 -->

## Welche Kosten fallen einmalig an?

Einmalig bezahlen Sie die Infrastruktur und je eine Daten-Pipeline pro Quelle.

**Die Infrastruktur** umfasst eigene Zugänge zu Sprachmodellen, eine durchsuchbare Wissensbasis aus Ihren Dokumenten, ein Rechte- und Rollenmodell und abgesicherte Speicher. <!-- K6 --> Der Aufbau kostet 4.000 bis 10.000 €. <!-- K1 -->

**Eine Daten-Pipeline** bringt Ihr Wissen in diese Wissensbasis. Für jede Quelle, etwa ein Wiki, ein Ticketsystem oder eine Sammlung von PDF-Handbüchern, entsteht eine eigene Verbindung. Sie bereinigt die Inhalte, teilt sie in sinnvolle Abschnitte, ergänzt Metadaten und aktualisiert alles täglich. <!-- K7 --> Pro Quelle kostet das 5.000 bis 8.000 €. <!-- K2 -->

Die Oberfläche, mit der Ihre Mitarbeitenden Fragen stellen, kann Ihr eigenes Team mit Copilot Studio bauen. Dann fallen dafür keine Projektkosten an. Entwickelt Insight AI die Anwendung, wird sie separat kalkuliert. <!-- K5 -->

## Was kostet das Sprachmodell jeden Monat?

Das Sprachmodell wird bei Azure OpenAI im Standardmodell nach Verbrauch abgerechnet. Sie zahlen pro verarbeitetem Textstück (Token), getrennt nach Frage und Antwort. <!-- F1 --> Bei hoher, gleichmäßiger Nutzung lässt sich stattdessen feste Kapazität reservieren, monatlich oder jährlich, mit planbaren Kosten. <!-- F2 -->

Diese Kosten rechnet Microsoft direkt mit Ihnen ab, auf derselben Rechnung wie Ihre übrigen Azure-Dienste. <!-- K8 --> [OFFEN: Typische Größenordnung der monatlichen Azure-Kosten aus bisherigen Projekten]

## Gibt es Kosten, auch wenn niemand fragt?

Ja, bei der Dokumentensuche. Azure AI Search berechnet im üblichen Modell reservierte Kapazität pro Stunde, unabhängig davon, wie viele Fragen gestellt werden. <!-- F4 --> Dieser Posten läuft also auch an Tagen weiter, an denen niemand den Assistenten nutzt. Beenden lässt er sich nur, indem man den Suchdienst löscht. <!-- F5 --> Microsoft bietet zusätzlich ein nutzungsabhängiges Modell an, das im Leerlauf nur den Speicher berechnet. Es befindet sich allerdings noch in der Vorschau. <!-- F6 -->

Die Betreuung durch Insight AI ist ebenfalls ein fester Monatsposten, ab 2.000 €. Sie lässt sich herunterfahren, wenn gerade nichts ansteht. <!-- K3 -->

## Rechenbeispiel

Ein Unternehmen will seinem Support einen Assistenten geben, der aus dem internen Wiki und dem Ticketsystem antwortet. Die Werte sind Annahmen innerhalb der veröffentlichten Preisspannen. <!-- K1 K2 --> Alle Preise in diesem Artikel verstehen sich zuzüglich Umsatzsteuer. <!-- K10 -->

| Posten | Annahme | Einmalig |
|---|---|---|
| Infrastruktur | mittlerer Umfang | 8.000 € |
| Pipeline Wiki | gut strukturierte Quelle | 6.000 € |
| Pipeline Ticketsystem | aufwendigere Quelle | 7.000 € |
| Oberfläche | eigenes Team mit Copilot Studio | keine Projektkosten |
| **Summe** | | **21.000 €** |

Damit liegt das Beispiel in der Spanne eines typischen Erstprojekts. <!-- K4 --> Monatlich kommen der Azure-Verbrauch und gegebenenfalls die Betreuung hinzu.

## Wovon hängt der Preis ab?

Den Preis bestimmen vor allem drei Dinge.

1. **Die Zahl der Datenquellen.** Jede Quelle ist eine eigene Pipeline. <!-- K2 -->
2. **Der Zustand der Daten.** Doppelte, veraltete oder schlecht strukturierte Inhalte machen die Aufbereitung aufwendiger. <!-- K7 --> [OFFEN: Thomas, welcher Faktor wird am häufigsten unterschätzt?]
3. **Datenschutz und Rechte.** Sollen personenbezogene Angaben vor der Verarbeitung entfernt werden, kommt ein Schritt hinzu. <!-- K7 --> Ein feines Rechtemodell sorgt dafür, dass niemand über den Assistenten Dokumente sieht, die er sonst nicht sehen darf. <!-- K6 -->

## Wann lohnt sich ein eigener Assistent nicht?

Ein eigener Assistent passt nicht, wenn Ihr Wissen vor allem in den Köpfen einzelner Mitarbeitender steckt und nicht in Dokumenten, Tickets oder Datenbanken. Er passt auch dann schlecht, wenn nur wenige Personen gelegentlich Fragen haben. Denn die Suche kostet im üblichen Modell auch ohne Nutzung Geld. <!-- F5 --> In beiden Fällen ist es günstiger, zuerst die Dokumentation zu verbessern.

## Aus der Praxis

Bei der Softengine Gruppe durchsucht der Assistent enGPT über 15.000 Dokumente, täglich aktualisiert, und beantwortet Fragen mit Quellenangaben. Er ist seit 1,5 Jahren produktiv im Einsatz. <!-- K9 --> [OFFEN: Was hat sich bei Softengine im Alltag am stärksten verändert?]

## Häufige Fragen

**Kann ich klein anfangen?**
Ja. Mit einer einzigen Quelle und einer Oberfläche aus Copilot Studio bleiben die Einmalkosten am unteren Ende der Spannen. <!-- K1 K2 K5 --> Weitere Quellen lassen sich später ergänzen.

**Verlassen meine Daten die EU?**
Nicht, wenn das Sprachmodell als „Data Zone Standard" für die EU bereitgestellt wird. Dann verarbeitet Microsoft die Daten innerhalb der EU-Datengrenze, gespeicherte Daten bleiben in der gewählten Azure-Region. <!-- F3 -->

**Gehören Code und Daten mir?**
Ja. Insight AI entwickelt direkt in Ihrer Azure- und GitHub-Umgebung. Code, Infrastruktur und Dokumentation bleiben bei Ihnen. <!-- K11 -->

## Nächster Schritt

In einem 45-minütigen Erstgespräch klären wir, welche Quellen Sie anbinden wollen und in welcher Spanne Ihr Projekt voraussichtlich liegt. [Termin vereinbaren](https://calendly.com/insightai/45min)

## Quellen
- Microsoft: [Azure OpenAI – Preise](https://azure.microsoft.com/de-de/pricing/details/cognitive-services/openai-service/) (abgerufen 25.09.2026)
- Microsoft Learn: [Deployment types for Foundry Models](https://learn.microsoft.com/en-us/azure/ai-foundry/foundry-models/concepts/deployment-types) (Stand 12.08.2026)
- Microsoft Learn: [Plan and manage costs of an Azure AI Search service](https://learn.microsoft.com/en-us/azure/search/search-sku-manage-costs) (Stand 02.07.2026)

## Bild
`visual.svg` · Alt-Text: Rechenbeispiel KI-Assistent: 21.000 € einmalig aus Infrastruktur und zwei Daten-Pipelines, dazu laufende Azure-Kosten.
