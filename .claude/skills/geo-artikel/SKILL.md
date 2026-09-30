---
name: geo-artikel
description: Aufbau von Fachartikeln, die bei Google gut ranken und von KI-Assistenten (ChatGPT, Perplexity, Copilot, Google AI Overviews) als Quelle zitiert werden. Laden, bevor ein Artikel gegliedert, geschrieben oder auf Auffindbarkeit geprüft wird.
user-invocable: false
---

# Artikel für Suchmaschinen und KI-Assistenten

Angelehnt an die Snippet-Regeln des Agenten `seo-snippet-hunter` (wshobson/agents, MIT), erweitert um Generative Engine Optimization (GEO). Leitidee: KI-Assistenten zitieren Abschnitte, die eine Frage allein und eindeutig beantworten, von einer Quelle mit erkennbarer Erfahrung.

## Pflichtaufbau

```markdown
---
titel: "<Frage oder klare Aussage, max. 60 Zeichen>"
meta_beschreibung: "<max. 155 Zeichen, enthält die Hauptfrage>"
hauptfrage: "<die eine Frage, die der Artikel beantwortet>"
nebenfragen:            # 3–6 verwandte Fragen, jede in Anführungszeichen
  - "<Frage 1>"
  - "<Frage 2>"
zielgruppe: <Rolle aus kontext/zielgruppe.md>
stand: <JJJJ-MM-TT>
---

# <Titel>

<Kurzantwort: 40–60 Wörter, beantwortet die Hauptfrage vollständig ohne Vorwissen>

## <Nebenfrage 1 als Überschrift>
<Antwort im ersten Satz, dann Erklärung, dann Beispiel>
...
## Wann das nicht passt
## Aus der Praxis   (nur freigegebene Beispiele)
## Häufige Fragen   (3–5 Fragen, je 2–3 Sätze)
## Nächster Schritt (ein Satz + Link zum Erstgespräch)
```

## Regeln

1. **Jeder Abschnitt steht für sich.** Keine Verweise wie „wie oben erwähnt". Ein KI-Assistent schneidet Abschnitte einzeln heraus.
2. **Antwort zuerst.** Unter jeder Frage-Überschrift beantwortet der erste Satz die Frage.
3. **Zahlen mit Einheit und Bezug.** „4.000–10.000 € einmalig für den Aufbau" statt „ein niedriger fünfstelliger Betrag".
4. **Tabellen für Vergleiche**, nummerierte Listen für Abläufe (5–8 Schritte).
5. **Begriffe definieren.** Jeder Fachbegriff bekommt beim ersten Auftreten einen Satz Erklärung, idealerweise als „X ist …".
6. **Erfahrung sichtbar machen.** Mindestens ein Satz, der nur von jemandem stammen kann, der das Projekt gemacht hat (freigegebenes Beispiel, typischer Fehler, echte Dauer). Das ist E-E-A-T und zugleich der Grund, warum ein Assistent gerade diese Quelle nennt.
7. **Quellen nennen.** Externe Fakten (Gesetze, Preise von Microsoft) mit Link am Ende. Lieber Primärquelle als Blog.
8. **Stand angeben.** Preise, Gesetze und Produkte ändern sich. `stand:` im Kopf und „Stand: Monat Jahr" im Text bei Preisangaben.
9. **Länge.** 900–1.500 Wörter. Lieber zwei Artikel als einer, der drei Hauptfragen beantwortet.

## Selbstprüfung (für den Stil- und den Fakten-Prüfer)
- [ ] Kurzantwort beantwortet die Hauptfrage ohne den Rest des Artikels
- [ ] Jede H2 ist eine Frage oder eine klare Aussage
- [ ] Erster Satz unter jeder H2 beantwortet sie
- [ ] Abschnitt „Wann das nicht passt" vorhanden
- [ ] FAQ mit 3–5 Einträgen
- [ ] Alle Zahlen haben eine Quelle in `02-recherche.md` oder `kontext/`
- [ ] Meta-Beschreibung ≤ 155 Zeichen, Titel ≤ 60 Zeichen

## Messen, ob KI-Assistenten uns nennen
Für jeden veröffentlichten Artikel die Hauptfrage und zwei Nebenfragen monatlich in ChatGPT, Perplexity und Copilot stellen. In `auswertung/metriken.csv` eintragen, ob insightai.co genannt oder verlinkt wird (Spalte `ki_nennung`).
