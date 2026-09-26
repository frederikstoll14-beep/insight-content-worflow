# Faktencheck
Ergebnis: NACHARBEIT NÖTIG

Runde 2, Stand 26.09.2026. Geprüft: `05-artikel.md` gegen `02-recherche.md`, `kontext/unternehmen.md`, `kontext/freigaben.md`.

**Erneute Prüfung der Quellen:** Der Egress-Proxy sperrt weiterhin bitkom.org, adoption.microsoft.com, getpanto.ai, hr-werkstatt.de, resources.ironmountain.com, copilotenschule.de, innogpt.de, snutig.de, kigen-it.de, marconomy.de und insightai.co. Erreichbar war wieder nur `microsoft.com/en-us/microsoft-365-copilot/copilot-adoption-guide`. Dort gibt es keine feste Wochenzahl für Rollout oder Einführung. Die Seite verweist auf Onboarding-Material, einen „QuickStart wizard“ und „The Great Copilot Journey“, eine 30-tägige geführte Tour für einzelne Nutzer. Das ist keine Zeitangabe für die Einführung im Unternehmen. Alle anderen Zeilen bleiben auf dem Stand der Suchzusammenfassungen. Sie sind als „korrekt lt. Recherche, ungeprüft“ markiert.

Firmenaussagen, die ohne ID direkt durch `kontext/unternehmen.md` gedeckt sind, werden wie in Runde 1 als „korrekt (ID fehlt)“ geführt.

| Stelle (Zitat) | ID | Befund | Empfehlung |
|---|---|---|---|
| „Bis Ihr Team den Assistenten täglich nutzt, vergeht mehr Zeit.“ | F4, F6 | korrekt (sinngemäß) | Beide Belege betreffen Microsoft Copilot, nicht einen eigenen Assistenten. Als Schlussfolgerung ist die Aussage vertretbar. „deutlich“ ist wie empfohlen gestrichen. |
| „Die meisten Zahlen stammen aus Blogs von Anbietern und nennen keine Datenbasis.“ | F5–F10 | korrekt | ID ist ergänzt. |
| „Für einen klar abgegrenzten Anwendungsfall im Mittelstand nennt hr-werkstatt.de 4 bis 12 Wochen, für die unternehmensweite Umstellung 6 Monate bis 2 Jahre.“ | F7 | korrekt lt. Recherche, ungeprüft (Seite gesperrt) | Vor Veröffentlichung direkt prüfen. |
| Tabelle hr-werkstatt.de: „4–8 Wochen Bewertung, 4–12 Wochen für einen klar definierten Anwendungsfall, 6 Monate bis 2 Jahre gesamt“ | F7 | korrekt lt. Recherche, ungeprüft | Befund aus Runde 1 („je Anwendungsfall“) ist behoben. |
| Tabelle innogpt.de: „7 Tage Testphase, danach 4 Wochen Nutzung beobachten“, „ohne Anbindung an Ihre Unternehmensdaten“ | F9 | korrekt lt. Recherche, ungeprüft | – |
| Tabelle skill-sprinters.de: „4–8 Wochen Vorbereitung, danach 12–24 Monate Projektphase“ | F8 | korrekt lt. Recherche, ungeprüft | – |
| Tabelle skill-sprinters.de: „erste Ergebnisse **nach** 8–12 Wochen“ | F8 | abweichend (leicht) | Laut F8 sollen Quick Wins „**innerhalb** von 8–12 Wochen realisierbar“ sein. „innerhalb“ nennt eine Obergrenze, „nach“ eine Untergrenze. Die Aussage wird so stillschweigend umgedreht. Ändern zu „erste Ergebnisse innerhalb von 8–12 Wochen“. |
| Quellenliste: skill-sprinters.de verlinkt nur die Startseite | F8 | Hinweis | Wie in Runde 1: Konkrete Beitrags-URL nachtragen, sonst ist der Beleg nicht auffindbar. |
| Tabelle kigen-it.de: „Pilotgruppe in Woche 1–6“, Microsoft 365 Copilot | F5 | korrekt lt. Recherche, ungeprüft | Steht klar als Anbieterangabe da. Das ist mit dem Vermerk der Recherche („nicht als Fakt zitieren“) vereinbar. |
| Tabelle snutig.de: „Aufwand für einen komplexen Assistenten das 3- bis 5-Fache eines einfachen FAQ-Bots“ | F10 | korrekt lt. Recherche, ungeprüft | Befund aus Runde 1 („kostet“) ist behoben. |
| „Alle Werte in der Tabelle sind Selbstauskünfte einzelner Anbieter ohne genannte Studie (Stand: September 2026).“ | F5, F7–F10 | korrekt | – |
| „Microsoft selbst nennt in seinem Leitfaden zur Copilot-Einführung keine pauschale Wochenzahl.“ / „Auch Microsoft nennt dafür keine Wochenzahl.“ | F3 | korrekt (Direktabruf microsoft.com) | Die abrufbare Seite enthält keine Wochenzahl für die Einführung. Die 30-Tage-Tour gilt nur für das Lernen einzelner Nutzer. adoption.microsoft.com war gesperrt. Der Titel „Adoption Playbook“ in der Quellenliste passt nur bedingt zur abgerufenen Seite, dazu siehe Offene Punkte. Die Phasenmodell-Aussagen aus Runde 1 sind gestrichen, damit sind die dortigen F3-Befunde erledigt. |
| „ein organisatorischer Teil, dessen Dauer vor allem von Ihrem Haus abhängt“ | – | Einschätzung, keine Tatsachenbehauptung | Vertretbar. Die Zeitzusage aus Runde 1 („zeitlich zusagen kann“) ist entfernt. |
| „Grundgerüst in Ihrer eigenen Azure-Umgebung, in dem Sprachmodell, Dokumentensuche und Rechte zusammenlaufen. Code, Infrastruktur und Dokumentation bleiben bei Ihnen.“ | K8 | korrekt | Die Bestandteile sind durch `unternehmen.md`, Abschnitt KI-Infrastruktur, gedeckt. |
| Pipeline: „Verbindung zu genau einer Quelle, etwa einem Wiki oder einem Ticketsystem … Standardschnittstellen … bereinigt … Abschnitte … Metadaten … synchronisiert täglich ohne Handarbeit“ | K2 | korrekt | – |
| „Jede weitere Quelle ist eine eigene Pipeline und damit eigener Aufwand.“ / FAQ „Jede Quelle ist eine eigene Pipeline mit eigenem Aufwand.“ | K2 | korrekt | – |
| „Der Zustand Ihrer Daten kann die Dauer stark beeinflussen.“ | – | vertretbar (abgeschwächt) | Wie in Runde 1 empfohlen abgeschwächt. Das ist jetzt eine Möglichkeitsaussage, kein Vergleich mehr. |
| „Schätzungen zufolge liegen 80 bis 90 % der Informationen … unstrukturiert vor … Nur 33 % der deutschen Unternehmen wollen solche Daten für KI-Anwendungen aufbereiten.“ | F11 | korrekt lt. Recherche, ungeprüft (Iron Mountain gesperrt) | Sicherheit „mittel“. Offen bleibt, ob beide Zahlen aus Iron Mountain stammen. Laut F11 kommen die 80–90 % aus IDC-Sekundärquellen, die Quellenliste nennt aber nur Iron Mountain. Das Datum ist ungeklärt. |
| „Bevor wir auf Ihre Systeme zugreifen, stehen **immer** eine NDA und ein AVV.“ / „Ohne beide Verträge beginnt keine Anbindung.“ | K4 | korrekt | `unternehmen.md`: „Vor Zugang: NDA und AVV“. „immer“ steht so in K4. Thomas sollte es bestätigen (wie Runde 1). |
| „Die meistgenannten Hemmnisse in der Bitkom-Studie 2026 betreffen Recht, Wissen und Personal. Unter Unternehmen, die KI bereits nutzen, nennen je 53 % … 51 % Personalmangel.“ | F2 | korrekt lt. Recherche, ungeprüft (bitkom.org gesperrt) | Satz aus Runde 1 („selten in der Software“) ist entfernt, die Bitkom-Studie wird jetzt im Text genannt. Weiterhin offen ist die Grundgesamtheit: Beziehen sich die Hemmnisse auf KI-nutzende Unternehmen oder auf alle Befragten? Der Artikel legt sich auf „KI-nutzende“ fest. Vor Veröffentlichung bei Bitkom prüfen. |
| „Schmale Pilotprojekte liefern verlässlichere Ergebnisse als ein breiter Start.“ | F12 | korrekt lt. Recherche, ungeprüft | – |
| Checkliste Punkte 2, 4–7 (Verantwortliche je Quelle, Rechte, IT-Sicherheit/Datenschutz, Pilotgruppe, Messgröße) | – | Empfehlungen, keine Tatsachenbehauptungen | Die Microsoft-Zuschreibung aus Runde 1 ist entfernt. Punkt 4 ist als Anforderung formuliert, nicht als Produktversprechen. Das passt zum RBAC-Rechtemodell in `unternehmen.md`. |
| „79 % der befragten Unternehmen haben Copilot ausgerollt, aber nur 35,8 % … Die Zahlen stammen aus einem Blog, nicht von Microsoft.“ | F4 | korrekt lt. Recherche, ungeprüft (getpanto.ai gesperrt) | „deutet auf eine Lücke hin“ ist wie empfohlen abgeschwächt. |
| „reine Lizenzverteilung nach sechs Monaten rund 20 % aktive Nutzer, ein mehrwöchiges Training mit Pilotgruppe über 70 %. Eine Datenquelle nennt er nicht.“ | F6 | korrekt lt. Recherche, ungeprüft | – |
| „Schulungen je Fachbereich und eine eigene Session für die Geschäftsführung gehören bei uns zum Angebot.“ | K6 | korrekt | – |
| „Seit 2023 haben wir über 80 Mitarbeitende aus 8 Unternehmen geschult.“ | K11 | korrekt | `freigaben.md`: Status **frei**. |
| „wirbt etwa mit einer 7-tägigen Testphase und empfiehlt danach, einfache Assistenten vier Wochen lang zu beobachten, ausdrücklich ohne Anbindung an echte Unternehmensdaten“ | F9 | korrekt lt. Recherche, ungeprüft | – |
| „Eine Wissensbasis … aus der die KI ihre Antworten mit Quellenangabe bildet.“ | – | korrekt (ID fehlt) | Gedeckt durch `unternehmen.md` („Antworten mit Quellenangabe“, „Durchsuchbare Wissensbasis“). |
| „schätzt den Aufwand für 500 Fachfragen aus Produktdokumentation auf das 3- bis 5-Fache eines FAQ-Bots mit 20 Standardfragen“ | F10 | korrekt lt. Recherche, ungeprüft | – |
| „reicht ein Standardprodukt mit Testphase. Es ist schneller.“ | F9 | korrekt | „günstiger“ aus Runde 1 ist gestrichen. |
| „Bei der Softengine Gruppe durchsucht der Assistent enGPT über 15.000 Dokumente, täglich aktualisiert, und antwortet mit Quellenangaben. Er ist seit 1,5 Jahren produktiv im Einsatz.“ | K9 | korrekt | `freigaben.md`: Status **frei**, alle Details stehen im freigegebenen Umfang. Die Formulierung „jeden Tag weiter gepflegt“ aus Runde 1 ist entfernt. Eine Einführungsdauer wird nicht behauptet (K10), die Lücke ist als `[OFFEN]` markiert. |
| FAQ: „Am häufigsten genannt werden eine fehlende Strategie und ein zu breiter Umfang. Mehrere Fachartikel sehen in einem der beiden oder in beiden den Hauptgrund fürs Scheitern, nicht in der Technik.“ | F12 | korrekt lt. Recherche, ungeprüft | Befund aus Runde 1 ist behoben, jetzt werden beide Gründe genannt. |
| FAQ: „Weitere Quellen lassen sich an dieselbe Wissensbasis anschließen“ | – | korrekt (ID fehlt) | Gedeckt durch `unternehmen.md` (Pipelines je Quelle, eine gemeinsame Wissensbasis). |
| „Ein typisches Erstprojekt kostet 15.000 bis 25.000 € einmalig.“ | K3 | korrekt (nur gegen `unternehmen.md`, insightai.co gesperrt) | – |
| „Aufbau der Infrastruktur mit 4.000 bis 10.000 € einmalig. Jede Datenquelle kostet 5.000 bis 8.000 € einmalig.“ | K1, K2 | korrekt (nur gegen `unternehmen.md`) | „Darin stecken …“ aus Runde 1 ist entfernt. Der Widerspruch zum Erstprojekt ist offen als `[OFFEN]` markiert. |
| „Alle Preise zuzüglich Umsatzsteuer, Stand: September 2026.“ | – (Kommentar) | korrekt (ID fehlt) | Gedeckt durch `unternehmen.md`. Den HTML-Kommentar vor Veröffentlichung entfernen. |
| „wir betreuen den Assistenten laufend ab 2.000 € im Monat. Die Betreuung lässt sich herunterfahren, wenn nichts ansteht.“ | K7 | korrekt | – |
| „45-minütigen Erstgespräch“, Calendly-Link | – | korrekt (ID fehlt) | Gedeckt durch `unternehmen.md`. |

Gesetze: Im Artikel wird kein Gesetz zitiert. NDA und AVV erscheinen nur als Vertragsarten.
GitHub-Belege (`G`-Zeilen): In `02-recherche.md` gibt es keine.
Freigaben: Softengine/enGPT (frei) und KI-Schulungen (frei) werden im freigegebenen Umfang verwendet. Das anonyme Projekt mit den Prepaid-Stromzählern kommt nicht vor.
Versprechen gegenüber `unternehmen.md`: Kein Versprechen geht über `unternehmen.md` hinaus. Die Zeitzusage aus Runde 1 ist entfernt, die Dauer bleibt `[OFFEN]`.

## Offene Punkte für Thomas

1. **Einzige blockierende Korrektur:** In der Tabelle bei skill-sprinters.de muss „erste Ergebnisse nach 8–12 Wochen“ zu „erste Ergebnisse innerhalb von 8–12 Wochen“ werden (F8). Danach ist der Artikel aus Sicht des Faktenchecks freigabefähig, abgesehen von den Punkten 2 bis 5.
2. **`[OFFEN]`-Marker füllen oder streichen**, bevor der Artikel erscheinen kann: Dauer des technischen Aufbaus (Einleitung und Abschnitt „technischer Aufbau“), Richtwert je weitere Quelle, Erwartungen an die Geschäftsführung und häufigste Verzögerungen, Einführungsdauer von enGPT, Veränderungen bei Softengine nach dem Start, Umfang des typischen Erstprojekts (15.000–25.000 € gegenüber 9.000–18.000 € für Infrastruktur plus eine Quelle). Wenn neue Zahlen dazukommen, braucht es eine weitere Prüfung.
3. **Direktprüfung vor Veröffentlichung** (aus dieser Umgebung gesperrt): F2 (Bitkom, inklusive Grundgesamtheit der Hemmnis-Zahlen), F7 (hr-werkstatt.de), F11 (Iron Mountain: welche Zahl aus welcher Quelle, Datum), außerdem F4–F6, F8–F10 und F12. Die Preise sind nur gegen `kontext/unternehmen.md` (Stand 25.09.2026) geprüft, nicht gegen insightai.co.
4. **Microsoft-Quelle:** Die Aussage „keine pauschale Wochenzahl“ ist für microsoft.com bestätigt. In der Quellenliste heißt der Link aber „Adoption Playbook“, obwohl die Seite eher eine Übersicht mit Onboarding-Material ist. Bitte prüfen, ob der Titel angepasst oder die Playbook-Seite auf adoption.microsoft.com verlinkt werden soll.
5. **„immer“ NDA und AVV** bitte bestätigen. Die skill-sprinters-URL auf den konkreten Beitrag ändern. Vor Veröffentlichung die HTML-Kommentare entfernen (Preiskommentar in der FAQ, „Hinweis für den Fakten-Prüfer“).

---

## Runde 1 (Kurzfassung)

Ergebnis damals: NACHARBEIT NÖTIG.

- **Ohne Beleg:** Zeitzusage „ein Dienstleister liefert in einem planbaren Zeitraum“ bzw. „zeitlich zusagen kann“, „vergeht deutlich mehr Zeit“, „Die meisten Zahlen stammen aus Blogs“ (ohne ID), „Zustand Ihrer Daten wirkt stärker als die Technik“, „Hemmnisse liegen selten in der Software“, vier Microsoft-Aussagen zu F3 (Phasenmodell, frühe Einbindung von IT/Security, Pilotphase, dauerhafte Begleitung), die der Direktabruf nicht bestätigte. **Stand Runde 2:** alle behoben (gestrichen, abgeschwächt oder mit ID versehen).
- **Abweichend:** hr-werkstatt „4–12 Wochen je Anwendungsfall“, snutig „kostet das 3- bis 5-Fache“, „schneller und günstiger“, Softengine „jeden Tag weiter gepflegt“, FAQ „Zu viel auf einmal wollen“ als alleiniger Hauptfehler, Erstprojekt „Darin stecken Infrastruktur und je Datenquelle“ (Rechnung geht nicht auf). **Stand Runde 2:** alle behoben. Der Erstprojekt-Umfang ist jetzt als `[OFFEN]` markiert.
- **Hinweise:** skill-sprinters nur als Startseite verlinkt (weiterhin offen), „immer“ bei NDA/AVV bestätigen (weiterhin offen), Grundgesamtheit der Bitkom-Hemmnisse klären (weiterhin offen), HTML-Kommentare entfernen (weiterhin offen).

## Nachtrag nach Runde 2
F8 (skill-sprinters.de) korrigiert: „nach 8–12 Wochen" → „innerhalb von 8–12 Wochen", wie in 02-recherche.md. Mit dem Menschen abgestimmt, kein dritter Prüflauf. Die übrigen offenen Punkte oben bleiben bis STOPP B bestehen.
