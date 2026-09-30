# Stilprüfung: 03-entwurf.md
Profil: `blog` · Grundlage: avoid-ai-writing + insight-stimme/deutsche-ki-muster

## Funde

| # | Stelle (Zitat) | Kategorie | Schwere |
|---|---|---|---|
| 1 | „Eine einzige Seite zeigt die Spannweite bereits: Für einen klar abgegrenzten Anwendungsfall im Mittelstand nennt hr-werkstatt.de 4 bis 12 Wochen, für die unternehmensweite Umstellung 6 Monate bis 2 Jahre." | Doppelpunkt-Einleitung + Satz mit ca. 29 Wörtern | klar |
| 2 | „Es empfiehlt stattdessen Phasen: Bereitschaft prüfen, mit einer Pilotgruppe starten, schrittweise ausweiten, die Nutzung dauerhaft begleiten." | Vierer-Kette in einem Satz, schwer lesbar | Ermessen |
| 3 | „Schmale Pilotprojekte liefern verlässlicher Ergebnisse als ein breiter Start." | Grammatikfehler (richtig: „verlässlichere") | klar |
| 4 | „Ein eigener Assistent mit Ihrer Wissensbasis passt nicht, wenn in den ersten Wochen niemand im Haus Zeit hat, Fragen zu Datenquellen zu beantworten und Rückmeldungen aus der Pilotgruppe zu sammeln." | Satz mit ca. 30 Wörtern, über der 25-Wörter-Grenze | klar |
| 5 | Drei „wenn"-Sätze in Folge im Abschnitt „Wann das nicht passt" (zwei davon im selben Absatz) | Rhythmus: gleiche Satzform wiederholt | Ermessen |
| 6 | „Ein technisch fertiger Assistent ist noch kein genutzter Assistent." | Antithese-Muster („A ist noch kein B"), leicht formelhaft | Ermessen |
| 7 | Abschnitt „Wie lange dauert der technische Aufbau?": fünf Absätze mit fast identischem Aufbau (Begriff erklären → Beispiel → Folge) | Rhythmus, Absatzlänge gleichförmig | Ermessen |
| 8 | Kein Stufe-1- oder Stufe-2-Wort in Häufung gefunden (kein „nahtlos", „Gamechanger", „Mehrwert generieren" o. Ä.) | Vokabular | — (kein Fund) |

## Änderungen
- Fund 1: Doppelpunkt aufgelöst, Satz in zwei Sätze geteilt. Fakten-ID F7 unverändert.
- Fund 2: Vierer-Kette in zwei Sätze geteilt („… mit einer Pilotgruppe starten. Danach schrittweise ausweiten …"), keine Aussage geändert. F3 unverändert.
- Fund 3: Tippfehler „verlässlicher" zu „verlässlichere" korrigiert. Keine inhaltliche Änderung, F12 unverändert.
- Fund 4: Satz geteilt in „… niemand im Haus Zeit hat." + „Jemand muss Fragen zu Datenquellen beantworten und Rückmeldungen aus der Pilotgruppe sammeln, sonst …". Ursprüngliche Kausalkette (Technik steht bereit, Zeitplan verschiebt sich) blieb erhalten, nur an den zweiten Satz angehängt.
- Fund 5: Letzten Absatz umgebaut. Aus „Und wenn Sie nur ausprobieren wollen … ist ein Standardprodukt … schneller und günstiger" wurde „Wollen Sie nur ausprobieren, ob Ihr Team mit KI-Chats arbeiten mag, reicht ein Standardprodukt mit Testphase. Es ist schneller und günstiger." Verb-Erst-Konstruktion statt drittem „wenn", Aussage unverändert, Nebensatz zusätzlich in eigenen Satz geteilt.
- Fund 6: bewusst nicht geändert. Die Antithese spiegelt die Überschrift direkt und trägt eine eigene, überprüfbare Aussage (Ausrollen vs. Nutzung) statt einer leeren Floskel.
- Fund 7: nicht strukturell umgebaut, da jeder Absatz einen eigenen Fakt behandelt (Infrastruktur, Pipeline, Datenzustand, Verträge) und ein Zusammenlegen Inhalte verändert hätte. Satzlängen innerhalb der Absätze variieren bereits (siehe zweiter Durchgang).
- Alle Fakten-Kommentare (`<!-- F… -->`, `<!-- K… -->`) und `[OFFEN: …]`-Stellen unverändert übernommen. Keine Zahl geändert.

## Zweiter Durchgang über die eigene Fassung
- Durchschnittliche Satzlänge geschätzt: rund 15–16 Wörter pro Satz. Nach der Teilung ist kein Satz mehr über 25 Wörter (längster jetzt ca. 24 Wörter: „Nach seiner Angabe erreicht reine Lizenzverteilung nach sechs Monaten rund 20 % aktive Nutzer, ein mehrwöchiges Training mit Pilotgruppe über 70 %.", unverändert aus dem Entwurf, F6).
- Kein neuer Gedankenstrich, keine neue Doppelpunkt-Einleitung eingeführt.
- Absatzlängen bleiben im Abschnitt „Wie lange dauert der technische Aufbau?" ähnlich (2–4 Sätze); das ist Ermessensfrage 7 und wurde bewusst so belassen, da eine Zusammenlegung Fakten vermischt hätte.
- Keine Stufe-1- oder Stufe-2-Häufung in der überarbeiteten Fassung gefunden.
- Rhetorische Fragen kommen nur als H2-Überschriften vor (zulässig laut `insight-stimme`, echte Fragen, keine Wortspiele), nicht als Übergänge im Fließtext.
- Wortzahl 05-artikel.md (Fließtext ohne Frontmatter, Kommentare und Quellenliste): rund 1.020 Wörter.

## Runde 2 (nach Faktencheck Runde 1)

Geprüft wurden nur die vom Autor nach dem Faktencheck geänderten Absätze (Liste des Rechercheurs). Übergänge nach den Kürzungen wurden geprüft und tragen; keine Fakten-ID, keine Zahl und keine [OFFEN]-Stelle wurde angefasst.

| # | Stelle (Zitat vorher) | Kategorie | Schwere | Änderung |
|---|---|---|---|---|
| 1 | „IT-Sicherheit, Datenschutz und IT früh einbinden." | Redundanz: „IT" taucht zweimal auf (in „IT-Sicherheit" und als eigener Punkt) | klar | Zu „IT-Sicherheit und Datenschutz früh einbinden." gekürzt. Keine Zuständigkeit gestrichen, nur die Dopplung entfernt. |
| 2 | „Eine Statistik-Auswertung zu Microsoft Copilot deutet darauf hin: 79 % der befragten Unternehmen haben Copilot ausgerollt, aber nur 35,8 % der lizenzierten Mitarbeitenden nutzen es aktiv." | Doppelpunkt-Einleitung + Satz mit 26 Wörtern, über der 25-Wörter-Grenze | klar | Doppelpunkt aufgelöst und Satz geteilt: „… deutet auf eine Lücke hin. 79 % der befragten Unternehmen …". Hedge „deutet … hin" blieb erhalten, F4 unverändert, beide Zahlen unverändert. |
| 3 | „Zwei Fehler werden besonders oft genannt: eine fehlende Strategie und ein zu breiter Umfang." | Doppelpunkt-Einleitung (gleiches Muster wie Fund 1 aus Runde 1) | klar | Zu „Am häufigsten genannt werden eine fehlende Strategie und ein zu breiter Umfang." umformuliert, ein Satz statt Doppelpunktliste. F12 unverändert, Aussage unverändert. |

Geprüft und unverändert gelassen, weil Übergänge tragen und keine 25-Wörter-Grenze verletzt wird:
- Einleitung unter H1: Übergang von „Bis Ihr Team den Assistenten täglich nutzt, vergeht mehr Zeit." zu „Diesen Teil bestimmen Sie selbst …" bezieht sich eindeutig auf den organisatorischen Teil, kein Bruch.
- Tabelle hr-werkstatt/snutig und die beiden Folgeabsätze: „Es gibt einen technischen Teil … Und es gibt einen organisatorischen Teil …" ist eine bewusste Zweiteilung, keine leere Wiederholung.
- „Der Zustand Ihrer Daten …": Übergang von der 33-%-Zahl (F11) zum Handbuch-Beispiel ist ein Sprung von Statistik zu Beispiel, aber inhaltlich schlüssig (beides zeigt: Datenaufbereitung ist Menschensache), kein Zusatzwort nötig.
- Geschäftsführung, 1. Absatz und Listenpunkt 6: Übergang von „keine Technik" zu den Bitkom-Zahlen (Recht, Wissen, Personal) passt inhaltlich, Punkt 6 unverändert kurz wie die übrigen Listenpunkte.
- „Warum ist ein Assistent …", 2. Absatz: Satz mit F6 bleibt bei ca. 22 Wörtern, unter der Grenze, aus Runde 1 unverändert übernommen.
- „Wann das nicht passt", 3. Absatz: dritter „Wenn"-Satz plus „Es ist schneller." als Kurzsatz nach Streichung von „und günstiger" – Übergang trägt, keine Lücke.
- „Aus der Praxis" (Softengine) und beide Kosten-FAQ: keine über 25 Wörter, keine Doppelpunkt- oder Floskel-Muster gefunden.

### Zweiter Durchgang (Runde 2)
- Alle drei neuen Sätze liegen jetzt unter 25 Wörtern (längster neuer Satz: 19 Wörter).
- Keine neue Doppelpunkt-Einleitung, kein neuer Gedankenstrich eingeführt.
- Keine Stufe-1/Stufe-2-Vokabelhäufung in den geänderten Stellen.
- Zahl der Änderungen in Runde 2: 3.
