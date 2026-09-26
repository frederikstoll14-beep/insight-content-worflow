---
name: artikel
description: Startet den kompletten Artikel-Ablauf von Insight AI für ein Thema oder eine Kundenfrage (Briefing, Recherche, Entwurf, Stil, Faktencheck, Grafik) mit zwei menschlichen Freigaben.
disable-model-invocation: true
argument-hint: <Thema, Kundenfrage oder Nummer aus dem Themenpool>
arguments: [thema]
---

# /artikel

Heute: !`date +%F`

Thema: **$ARGUMENTS**

Du bist der Chefredakteur. Du schreibst selbst nichts, sondern steuerst die Agenten, prüfst ihre Dateien und hältst an den Stopps an.

## 0 · Vorbereiten
1. Ist das Thema eine Nummer (z. B. `T3`), lies den Eintrag aus `themen/themenpool.md`.
2. Bilde einen kurzen Slug (Kleinbuchstaben, Bindestriche, ohne Umlaute) und lege `content/<heute>-<slug>/` an.
3. Lege eine Aufgabenliste mit den Schritten 1–6 an.

## 1 · Briefing
Starte den Agenten **themen-scout** (Modus 1) mit Thema und Laufordner. Prüfe, dass `01-briefing.md` alle Felder hat.

## 2 · Recherche
Starte **rechercheur** mit dem Laufordner. Prüfe, dass `02-recherche.md` Primärquellen enthält und jede Zeile eine ID hat.

## ⏸ STOPP A
Zeige dem Menschen in fünf bis acht Zeilen
- Hauptfrage, Winkel, Zielrolle
- die drei wichtigsten Fakten mit Quelle
- alle `[OFFEN]`-Fragen an Thomas

Frage: „Passt die Richtung? Antworten auf offene Fragen jetzt ergänzen oder als [OFFEN] stehen lassen?" **Warte auf Antwort.** Trage Antworten von Thomas in `02-recherche.md` unter „Aus kontext/" mit der ID `T1`, `T2` … ein.

## 3 · Entwurf
Starte **autor** mit dem Laufordner.

## 4 · Stil
Starte **stil-pruefer** für `03-entwurf.md` (Profil `blog`). Ergebnis ist `05-artikel.md`.

## 5 · Faktencheck
Starte **fakten-pruefer** mit dem Laufordner. Er darf den Entwurfsverlauf nicht sehen, gib ihm deshalb nur den Pfad und keine Zusammenfassung.
- Bei NACHARBEIT NÖTIG: Gib die Befunde an **autor** zurück (nur die betroffenen Stellen korrigieren), danach erneut **stil-pruefer** nur für die geänderten Absätze und erneut **fakten-pruefer**. Höchstens zwei Runden, dann an den Menschen übergeben.

## 6 · Grafik
Starte **visual-designer** mit dem Laufordner.

## ⏸ STOPP B
Gib aus
- Pfad zu `05-artikel.md` und `visual.svg`
- Wortzahl, Ergebnis des Faktenchecks, Zahl der verbleibenden `[OFFEN]`
- einen Satz, was an diesem Artikel am ehesten angreifbar ist

Setze den Status im Themenpool auf `zur Freigabe`. Nach Freigabe durch Thomas: Status `freigegeben` und `/linkedin <Laufordner>` vorschlagen.
