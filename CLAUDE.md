# Insight AI Content-Flow

Dieses Projekt erzeugt Fachartikel für insightai.co und LinkedIn-Beiträge für Thomas Weller. Ziel ist, dass mittelständische Unternehmen über Google, LinkedIn und Antworten von KI-Assistenten auf Insight AI aufmerksam werden.

## Grundregeln

1. **Nichts erfinden.** Keine Kundennamen, Projektzahlen, Zitate oder Preise, die nicht in `kontext/` oder in einer geprüften Quelle stehen. Fehlt etwas, schreibe `[OFFEN: …]` in den Text statt einer Annahme.
2. **Kundendaten sind vertraulich.** Nur Projekte und Zahlen verwenden, die in `kontext/freigaben.md` als freigegeben markiert sind.
3. **Jeder Schritt schreibt eine Datei.** Agenten übergeben Ergebnisse über Dateien im Laufordner, nie nur im Chat. So bleibt jeder Lauf nachvollziehbar und versionierbar.
4. **Menschen geben frei.** Der Ablauf stoppt an zwei Stellen und wartet auf ein OK (siehe unten). Veröffentlicht wird nie automatisch.
5. **Sprache.** Deutsch, Anrede „Sie" auf der Website, „Sie" oder neutral auf LinkedIn (siehe Skill `insight-stimme`).

## Ablauf

```
/themen  →  themen/themenpool.md
/artikel <Thema oder Kundenfrage>
   1 themen-scout     → 01-briefing.md
   2 rechercheur      → 02-recherche.md
   ── STOPP A: Mensch prüft Briefing und Recherche ──
   3 autor            → 03-entwurf.md
   4 stil-pruefer     → 04-stil.md + 05-artikel.md
   5 fakten-pruefer   → 06-faktencheck.md   (sieht nur Artikel und Recherche)
   6 visual-designer  → visual.svg
   ── STOPP B: Freigabe durch Thomas ──
/linkedin <Laufordner>  → linkedin.md
/auswertung             → auswertung/learnings.md
```

Laufordner: `content/JJJJ-MM-TT-<slug>/`

## Wo was liegt

| Ordner | Inhalt |
|---|---|
| `kontext/` | Fakten über Insight AI, Zielgruppe, Freigaben. Einzige Quelle für Firmenaussagen. |
| `themen/` | Themenpool mit Status |
| `content/` | Ein Ordner pro Lauf mit allen Zwischenständen |
| `auswertung/` | Kennzahlen (CSV) und daraus gezogene Learnings |
| `.claude/agents/` | Die Spezialisten |
| `.claude/skills/` | Wissen (Stimme, GEO, LinkedIn, Anti-KI-Stil) und die Befehle `/artikel`, `/linkedin`, `/themen`, `/auswertung` |

## Firmen-GitHub von Insight AI (geplant, noch kein Zugriff)

Der Ablauf bekommt Lesezugriff auf das Unternehmens-GitHub von Insight AI. Dann beantwortet der Rechercheur viele Fragen an Thomas selbst, zum Beispiel Projektdauer aus der Commit-Historie, Ablauf aus Projektdokus und Zahl der Datenquellen aus der Infrastruktur.

- **Solange kein Zugriff besteht**, bleiben diese Fragen `[OFFEN]` und bekommen den Zusatz „(per Firmen-GitHub klärbar)".
- **Sobald Zugriff besteht**, gilt: Aussagen aus GitHub bekommen die ID `G1`, `G2` … mit Repo und Datei, Commit oder Issue als Beleg. Sie gelten als Firmenquelle wie `kontext/`.
- **Grundregel 2 gilt weiter.** Kundennamen, Projektnamen und Zahlen aus einem Kundenrepo nur verwenden, wenn das Projekt in `kontext/freigaben.md` freigegeben ist. Sonst nur anonym („ein Kunde aus dem Maschinenbau") oder gar nicht.
- **Nur lesen.** Im Firmen-GitHub wird nichts geändert, kommentiert oder angelegt.
- **Keine Interna.** Keine Secrets, Zugangsdaten, internen Hostnamen, Preise aus Angeboten oder Code-Ausschnitte in Artikel übernehmen.
- **Was nicht im Code steht, bleibt bei Thomas.** Einschätzungen, Erfahrungen aus Gesprächen und Zitate kann GitHub nicht liefern. An STOPP A prüft der Mensch weiterhin alle `G`-Zeilen.

## Wenn du `learnings.md` änderst

Neue Erkenntnisse aus der Auswertung gehören in `auswertung/learnings.md`. Die Agenten lesen diese Datei vor jedem Lauf. Regeln dort haben Vorrang vor den allgemeinen Skills, aber nicht vor den Grundregeln oben.
