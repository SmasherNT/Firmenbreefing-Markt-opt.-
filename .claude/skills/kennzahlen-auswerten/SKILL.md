---
name: kennzahlen-auswerten
description: Anleitung zur Erhebung und Berechnung von Finanzkennzahlen aus Jahresabschlüssen und Geschäftsberichten für Firmenbriefings. Verwenden bei jeder Finanzanalyse eines Unternehmens.
---

# Kennzahlen auswerten

## Basisdaten (je Geschäftsjahr, je Wert ein Claim `C-F..` mit Belegstelle)
Umsatz · EBITDA · EBIT · Jahresüberschuss · Bilanzsumme · Eigenkapital · Finanzverbindlichkeiten ·
liquide Mittel · operativer Cashflow · Investitionen (Capex) · Mitarbeitende

## Kennzahlen
| Kennzahl | Formel |
|---|---|
| Umsatzwachstum | (Umsatz t / Umsatz t-1) − 1 |
| EBITDA-Marge | EBITDA / Umsatz |
| EBIT-Marge | EBIT / Umsatz |
| Nettomarge | Jahresüberschuss / Umsatz |
| Eigenkapitalquote | Eigenkapital / Bilanzsumme |
| Nettoverschuldung | Finanzverbindlichkeiten − liquide Mittel |
| Verschuldungsgrad | Nettoverschuldung / EBITDA |
| Free Cashflow | operativer Cashflow − Capex |
| Umsatz je Mitarbeitendem | Umsatz / Mitarbeitende |

Berechnungen mit `Bash` (z. B. `python3 -c`) nachvollziehbar durchführen; Ergebnisse auf eine Nachkommastelle runden.

## Pflichtangaben
- Rechnungslegung (HGB/IFRS/US-GAAP), Geschäftsjahresende, Konzern- oder Einzelabschluss, Währung
- Bestätigungsvermerk (uneingeschränkt/eingeschränkt/versagt)
- Sondereffekte und Vergleichbarkeitsbrüche

## Format `work/kennzahlen.md`
Claim-Register (Format siehe Skill `quellen-sichern`) → Tabelle Basisdaten (mit Claim-IDs) → Tabelle Kennzahlen
(Rechenweg, Claim-IDs der Eingangswerte) → Auffälligkeiten → Widersprüche, Stichtagsprobleme, Datenlücken.
Kleine Gesellschaften mit verkürztem Abschluss: verfügbare Werte nutzen, Rest „n. v.“.
