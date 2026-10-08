# Firmenbriefing-Workflow

Dieses Repository erstellt quellengestützte Firmenbriefings mit Markt- und Wettbewerbseinordnung.
Grundlage jeder Analyse ist der Auftrag in `input/auftrag.md`.

## Verzeichnisse

| Pfad | Zweck |
|---|---|
| `input/auftrag.md` | Auftrag: Zielunternehmen, Fragestellung, Umfang, Frist |
| `work/` | Zwischenergebnisse (Quellenliste, Rohnotizen, Kennzahlen, Teilanalysen) |
| `output/` | Fertiges Briefing (`output/briefing-<firma>-<JJJJ-MM-TT>.md`) |
| `.claude/agents/` | Spezialisierte Subagenten |
| `.claude/skills/` | Wiederverwendbare Arbeitsanleitungen |

## Ablauf

1. Auftrag lesen und offene Punkte klären (Skill `firmenbriefing`).
2. Quellen sammeln und sichern → `work/quellen.md` (Agent `quellen-recherche`, Skill `quellen-sichern`).
3. Finanzen auswerten → `work/kennzahlen.md` (Agent `finanz-analyse`, Skill `kennzahlen-auswerten`).
4. Markt und Wettbewerb einordnen → `work/markt.md` (Agent `markt-analyse`, Skill `markt-wettbewerb`).
5. Briefing schreiben → `output/` (Skill `briefing-schreiben`).
6. Fakten prüfen (Agent `faktenpruefung`), Befunde einarbeiten.

## Quellenregeln

- Vorrang haben öffentliche **Originalquellen**: Geschäfts- und Jahresberichte, Unternehmensregister/Bundesanzeiger,
  Handelsregister, Börsenpflichtmitteilungen (Ad-hoc, Stimmrechte), SEC/EDGAR, Investor-Relations-Seiten,
  amtliche Statistik (Destatis, Eurostat), Aufsichts- und Verbandsveröffentlichungen.
- Sekundärquellen (Presse, Datenbanken, Blogs) nur ergänzend und als solche gekennzeichnet.
- Jede Zahl und jede Tatsachenbehauptung bekommt eine Quelle mit URL, Titel, Herausgeber, Datum und Abrufdatum.
- Ist eine Originalquelle nicht abrufbar, das offen vermerken – keine Werte aus dem Gedächtnis ergänzen.
- Annahmen, Schätzungen und Bewertungen deutlich von belegten Fakten trennen.
- Keine personenbezogenen Daten über das Notwendige (Organe, Gesellschafter laut Register) hinaus.

## Werkzeuge

- `WebSearch` zum Auffinden von Quellen, `WebFetch` zum Lesen der Originaldokumente.
- Hinweis zur Cloud-Umgebung: Ist ein Host durch die Netzwerkrichtlinie gesperrt, den Host nennen;
  freigeben lässt er sich unter Umgebung → Bearbeiten → Netzwerkzugriff (Allowed domains).

## Stil

- Sprache: Deutsch, sachlich, knapp. Zahlen mit Einheit, Währung, Geschäftsjahr.
- Datumsformat TT.MM.JJJJ, Beträge in Mio. EUR, sofern der Auftrag nichts anderes vorgibt.
