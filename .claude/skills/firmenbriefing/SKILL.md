---
name: firmenbriefing
description: Steuert den gesamten Firmenbriefing-Workflow vom Auftrag in input/auftrag.md bis zum geprüften Briefing in output/. Verwenden, wenn ein Firmenbriefing, Unternehmensprofil oder eine Firmen- und Marktanalyse erstellt werden soll.
---

# Firmenbriefing – Gesamtablauf

## 1. Auftrag prüfen
- `input/auftrag.md` lesen. Pflichtfelder (Firmenname, Anlass, zentrale Fragen) müssen gefüllt sein.
- Fehlen Pflichtangaben oder ist das Unternehmen nicht eindeutig, nachfragen statt raten.

## 2. Arbeitsstand anlegen
- `work/status.md` mit Checkliste der Schritte 3–7 anlegen und laufend aktualisieren.

## 3. Quellen
- Agent `quellen-recherche` beauftragen → `work/quellen.md`.

## 4. Finanzen und Markt (parallel möglich)
- Agent `finanz-analyse` → `work/kennzahlen.md`
- Agent `markt-analyse` → `work/markt.md`

## 5. Briefing schreiben
- Skill `briefing-schreiben` anwenden → `output/briefing-<firma>-<JJJJ-MM-TT>.md`

## 6. Faktenprüfung
- Agent `faktenpruefung` beauftragen, alle Befunde „abweichend“/„unbelegt“ korrigieren oder streichen.

## 7. Abschluss
- Offene Punkte und nicht abrufbare Quellen im Briefing unter „Grenzen der Analyse“ nennen.
- Ergebnis committen.
