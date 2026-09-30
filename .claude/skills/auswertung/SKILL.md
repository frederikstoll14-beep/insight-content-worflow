---
name: auswertung
description: Wertet die Kennzahlen veröffentlichter Artikel und LinkedIn-Beiträge aus und leitet konkrete Regeln für die nächsten Inhalte ab.
disable-model-invocation: true
argument-hint: "[Zeitraum, z. B. letzte 30 Tage]"
allowed-tools: Read Write Edit Bash(python3 *)
---

# /auswertung

Zeitraum: **$ARGUMENTS** (Standard: alles seit der letzten Auswertung)

1. Lies `auswertung/metriken.csv`. Wenn weniger als drei Zeilen Kennzahlen haben, sage das und brich ab. Aus zu wenig Daten werden keine Regeln abgeleitet.
2. Rechne mit einem kurzen Python-Skript (keine Schätzung im Kopf)
   - LinkedIn: Engagement-Rate = (Reaktionen + Kommentare + Reposts) / Impressionen, je Format (A/B/C), Wochentag und Uhrzeit
   - Website: Klicks und Impressionen aus der Search Console, Verweildauer, Anfragen über das Erstgespräch
   - KI-Nennungen: Anteil der Testfragen, bei denen insightai.co genannt wird
3. Vergleiche mit der vorherigen Auswertung in `auswertung/learnings.md`.
4. Formuliere höchstens drei **neue Regeln**, jede mit Datengrundlage und Anzahl Beobachtungen, z. B. „Format C (Zahlen) erzielt 2,1-fache Engagement-Rate gegenüber A (n = 6 zu 5)". Markiere Regeln mit n < 5 als vorläufig.
5. Hänge die Auswertung mit Datum oben an `auswertung/learnings.md` an.
6. Schlage zwei Themen für den nächsten Monat vor und begründe sie mit den Daten.
