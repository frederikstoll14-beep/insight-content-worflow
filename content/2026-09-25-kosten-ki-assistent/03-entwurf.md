---
titel: Was kostet ein eigener KI-Assistent für Firmenwissen?
meta_beschreibung: Was ein KI-Assistent für Firmenwissen im Mittelstand kostet, einmalig und monatlich, und wovon der Preis abhängt. Mit Rechenbeispiel.
hauptfrage: Was kostet ein eigener KI-Assistent für unser Firmenwissen?
nebenfragen:
  - "Welche Kosten fallen einmalig an?"
  - "Was kostet das Sprachmodell?"
  - "Gibt es Kosten ohne Nutzung?"
  - "Wovon hängt der Preis ab?"
  - "Spart Selbstbauen Geld?"
zielgruppe: Geschäftsführung
stand: 2026-09-25
---

<!-- Gliederung
1 Kurzantwort · 2 Einmalig · 3 Laufend · 4 Rechenbeispiel · 5 Preistreiber · 6 Wann nicht · 7 Praxis · 8 FAQ · 9 Nächster Schritt
-->

# Was kostet ein eigener KI-Assistent für Firmenwissen?

In der heutigen schnelllebigen Welt ist künstliche Intelligenz für mittelständische Unternehmen von zentraler Bedeutung. Doch was kostet das eigentlich? Die Antwort: Ein typisches erstes Projekt kostet 15.000–25.000 € einmalig. <!-- K4 --> Hinzu kommen die nutzungsabhängigen Kosten bei Microsoft und optional eine Betreuung ab 2.000 € im Monat. <!-- K3 --> Es ist wichtig zu beachten, dass der größte Kostenfaktor nicht die KI selbst ist, sondern die Anbindung Ihrer Daten.

## Welche Kosten fallen einmalig an?

Die einmaligen Kosten bestehen aus zwei Bausteinen, die eine entscheidende Rolle spielen.

**Die Infrastruktur** ist das nahtlose Fundament des Assistenten. Sie umfasst eigene Zugänge zu Sprachmodellen, eine durchsuchbare Wissensbasis aus Ihren Dokumenten, ein Rechte- und Rollenmodell und abgesicherte Speicher. <!-- K6 --> Der Aufbau kostet 4.000–10.000 €. <!-- K1 -->

**Die Daten-Pipelines** sorgen dafür, dass Ihr Wissen in die KI kommt. Für jede Quelle – ob Wiki, Ticketsystem oder PDF-Handbücher – wird eine Verbindung gebaut, die Inhalte bereinigt, in sinnvolle Abschnitte teilt, mit Metadaten versieht und täglich aktualisiert. <!-- K7 --> Pro Quelle kostet das 5.000–8.000 €. <!-- K2 -->

Die Oberfläche selbst kann Ihr Team mit Copilot Studio bauen. Dann entstehen hier keine weiteren Projektkosten. Soll Insight AI die Anwendung entwickeln, wird sie separat kalkuliert. <!-- K5 -->

## Welche Kosten fallen jeden Monat an?

Laufend zahlen Sie zwei Dinge: den Verbrauch bei Microsoft Azure und, falls gewünscht, die Betreuung.

Das Sprachmodell wird bei Azure OpenAI im Standardmodell nach Verbrauch abgerechnet, also pro verarbeitetem Text (Tokens), getrennt nach Frage und Antwort. <!-- F1 --> Wer viel und gleichmäßig nutzt, kann stattdessen feste Kapazität reservieren und bekommt planbare Monatskosten. <!-- F2 -->

Die Suche über Ihre Dokumente (Azure AI Search) funktioniert anders. Im üblichen Modell zahlen Sie pro Stunde für reservierte Kapazität, egal wie viele Fragen gestellt werden. <!-- F4 --> Das bedeutet auch, dass Kosten entstehen, wenn niemand den Assistenten nutzt. <!-- F5 -->

Diese Kosten laufen direkt zwischen Ihnen und Microsoft, auf einer Rechnung. <!-- K8 --> [OFFEN: Typische Größenordnung der Azure-Kosten pro Monat aus bisherigen Projekten]

Die Betreuung durch Insight AI kostet ab 2.000 € im Monat und lässt sich herunterfahren, wenn nichts ansteht. <!-- K3 -->

## Rechenbeispiel

Ein Unternehmen möchte einen Assistenten für Support-Mitarbeiter, der aus dem internen Wiki und dem Ticketsystem antwortet.

| Posten | Annahme | Kosten |
|---|---|---|
| Infrastruktur | mittlerer Umfang | 8.000 € |
| Pipeline Wiki | einfache Quelle | 6.000 € |
| Pipeline Ticketsystem | aufwendigere Quelle | 7.000 € |
| Oberfläche | Team baut mit Copilot Studio | 0 € Projektkosten |
| **Einmalig gesamt** | | **21.000 €** |

Das ist ein Gamechanger für die Budgetplanung und liegt in der typischen Spanne von 15.000–25.000 €. <!-- K4 -->

## Wovon hängt der Preis ab?

Der Preis hängt vor allem von der Anzahl und Art der Datenquellen, der Datenqualität und den Anforderungen an Rechte und Datenschutz ab. Jede zusätzliche Quelle ist ein eigener Baustein. Unstrukturierte oder veraltete Daten machen die Aufbereitung aufwendiger. Sollen personenbezogene Angaben vorher entfernt werden, kommt ein Schritt hinzu. <!-- K7 --> Die Wahl des Sprachmodells ist dagegen meist ein kleinerer Faktor.

## Wann lohnt sich ein eigener Assistent nicht?

Ein eigener Assistent lohnt sich nicht, wenn Ihr Wissen nicht in Dokumenten, Tickets oder Datenbanken vorliegt. Er lohnt sich auch nicht, wenn nur wenige Personen gelegentlich Fragen haben. Dann rechnen sich die festen Kosten der Suche kaum.

## Aus der Praxis

Bei der Softengine Gruppe durchsucht der Assistent enGPT seit 1,5 Jahren über 15.000 Dokumente, die täglich aktualisiert werden. <!-- K9 --> Zusammenfassend lässt sich sagen, dass ein solches System nachhaltigen Mehrwert generiert. [OFFEN: Was hat Softengine am meisten überrascht, Aufwand oder Nutzen?]

## Häufige Fragen

**Kann ich klein anfangen?**
Ja. Mit einer Quelle und der Oberfläche aus Copilot Studio bleiben die Einmalkosten nahe am unteren Ende. <!-- K1 K2 K5 -->

**Verlassen meine Daten die EU?**
Mit dem Bereitstellungstyp „Data Zone Standard" für die EU werden Daten innerhalb der EU-Datengrenze verarbeitet. <!-- F3 -->

**Gehören Code und Daten mir?**
Ja, alles liegt in Ihrer eigenen Azure- und GitHub-Umgebung.

## Nächster Schritt

Die Zukunft ist spannend. In einem 45-minütigen Erstgespräch klären wir, welche Quellen Sie anbinden wollen und in welcher Spanne Ihr Projekt liegt: [Termin vereinbaren](https://calendly.com/insightai/45min)

## Quellen
- Microsoft: Azure OpenAI – Preise, https://azure.microsoft.com/de-de/pricing/details/cognitive-services/openai-service/
- Microsoft Learn: Deployment types, https://learn.microsoft.com/en-us/azure/ai-foundry/foundry-models/concepts/deployment-types
- Microsoft Learn: Plan and manage costs of an Azure AI Search service, https://learn.microsoft.com/en-us/azure/search/search-sku-manage-costs

---
Wortzahl ca. 780 · 2 × [OFFEN] · Fakten: F1–F5, K1–K9
