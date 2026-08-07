# Sprint-3-Plan — P1 „Mission Control 2.0" (PL)

*Erstellt 2026-08-07. Sprint-Motto: „Härtung + Abnahme" (P1-E4/E5 + G3). Basis: `p1-v0.2` (G4/D005), D006 (SMTP = S1, Einrichtung folgt).*

## Sprint-Ziel

P1 wird abnahmereif gegen die 5 Kriterien des Projektauftrags. Dieser Sprint ist bewusst **mensch-lastig**: Die verbleibenden Nachweise (SMTP-Aktivierung + erste echte DR-Mail, Copilot-PoC-Lauf, Geräte-Stichproben, Inbox-DR-Zähler) entstehen an deinem PC; ab jetzt laufen **alle Gates als Inbox-DRs** (Regelkanal, Kriterium 3).

## Sprint-Backlog

| # | Ticket | Inhalt | Rolle | Wartet auf |
|---|---|---|---|---|
| 1 | T-0016 | Retro-CR S2: Stichproben-Zeile + Zähler in Gate-Vorlagen | COACH | — |
| 2 | T-0017 | SMTP aktivieren (D006/S1: App-Passwort + setx) → erste echte DR-Mail als Nachweis | Mensch+DEV | App-Passwort |
| 3 | T-0018 | Copilot-PoC-Lauf p0/T-0072 am Team-Node (P0-Kriterium 9 voll) | Mensch+DEV | ~5 Min am PC |
| 4 | T-0019 | Geräte-Stichproben dokumentieren (D003 + D005: Selector, Übersicht, 3 neue Tabs) | Mensch | ~5 Min am PC |
| 5 | T-0020 | Abnahme-Review gegen Projektauftrag-Kriterien 1–5 → **G3 als Inbox-DR** | PL→Mensch | T-0017–T-0019 |
| 6 | T-0021 | Sprint-3-Report + Schluss-Retro → **G4 als Inbox-DR** | PL | T-0020 |

## Inbox-DR-Zähler (Kriterium 3: ≥5 in P1 inkl. E-Mail)

Stand: **1** (T-0014/D006). Geplant in diesem Sprint: G3-DR + G4-DR + Stichproben-Bestätigungs-DR + SMTP-Nachweis-DR → Ziel erreichbar; ab T-0017 mit echter E-Mail-Benachrichtigung je DR.

## Arbeitsweise

Session legt DRs an und pusht; du beantwortest in Mission Control (E-Mail kommt nach T-0017 automatisch); nächste Session verbucht und schließt. `abschluss.cmd` nach jeder Runde.
