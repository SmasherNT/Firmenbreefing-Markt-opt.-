---
name: quellen-sichern
description: Regeln und Format zum Finden, Prüfen und Dokumentieren öffentlicher Originalquellen für Firmenbriefings. Verwenden bei jeder Quellenrecherche und beim Zitieren.
---

# Quellen sichern

## Quellenhierarchie
1. **Register & Pflichtpublikationen:** Unternehmensregister, Bundesanzeiger, Handelsregister, Transparenzregister-Hinweise
2. **Unternehmenseigene Pflicht- und IR-Dokumente:** Geschäftsbericht, Jahresabschluss, Ad-hoc- und Stimmrechtsmitteilungen, Hauptversammlungsunterlagen
3. **Ausländische Pflichtpublikationen:** SEC/EDGAR (10-K, 20-F), Companies House, nationale Register
4. **Amtliche Statistik & Aufsicht:** Destatis, Eurostat, Bundesbank, BaFin, Kartellbehörden
5. **Verbände & Fachstudien** (als Sekundärquelle kennzeichnen)
6. **Presse & Datenbanken** (nur ergänzend, Sekundärquelle)

## Suchmuster
- `"<Firmenname>" Jahresabschluss <Jahr>` · `"<Firmenname>" Geschäftsbericht filetype:pdf`
- `"<Firmenname>" HRB` · `site:<firmen-domain> investor relations`
- Markt: `<Branche> Umsatz Destatis` · `<Branche> Marktvolumen Verband`

## Prüfung jeder Quelle
- Mit `WebFetch` öffnen; Aussage muss im Dokument stehen.
- Datum/Geschäftsjahr und Herausgeber notieren; Aktualität bewerten.
- Bei Sperre oder Fehler: Status `gesperrt`/`nicht erreichbar` + Host vermerken.

## Format `work/quellen.md`
| ID | Titel | Herausgeber | Typ | Datum | URL | Abruf | Kernaussage / Verwendung | Status |
|---|---|---|---|---|---|---|---|---|
| Q1 | … | … | Original | TT.MM.JJJJ | … | TT.MM.JJJJ | … | abrufbar |

Im Text wird mit `[Q1]` zitiert.
