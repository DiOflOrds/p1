# Sprint-2-Plan — P1 „Mission Control 2.0" (PL)

*Erstellt 2026-08-07. Sprint-Motto: „Views + Inbox-Regelkanal" (P1-E2 + E3). Basis: `p1-v0.1` (G4/D003).*

## Sprint-Ziel

Der Mensch sieht Requirements, Traceability und Baselines ohne Git-Zugriff im Frontend (P0-Kriterium-5-Rest), und die Decision-Inbox wird zum Regelkanal: E-Mail-Benachrichtigung bei jedem neuen DR (D004 endlich real), SMTP-Einrichtung als **erster echter P1-Inbox-DR** an den Menschen (B5-Zählung startet).

## Sprint-Backlog

| # | Ticket | Inhalt | Rolle | blocked_by |
|---|---|---|---|---|
| 1 | T-0010 | Retro-CR S1: `trace_matrix --alle-projekte` (SWR-Quellen per Discovery) | DEV | — |
| 2 | T-0011 | SWE.1: SWR-030–033 (Views + DR-Benachrichtigung) draft→reviewed → **G1** | RM | — |
| 3 | T-0012 | Views: Requirements/Traceability/Baselines (API + Frontend) | DEV | T-0011 |
| 4 | T-0013 | DR-Benachrichtigung: Skript, einmalig je DR, ausfalltolerant + Marker | DEV | T-0011 |
| 5 | T-0014 | **Inbox-DR an Mensch:** SMTP-Zugang einrichten (Optionen maschinenlesbar) | PL→Mensch | — |
| 6 | T-0015 | Verifikation SWR-030–033, Matrix, Report → **G4** | TEST | T-0012, T-0013 |

## Human-Gates

**G1** (SWR-030–033), **G4** (Review inkl. Stichprobe — auch die offene aus D003 kann dabei nachgeholt werden). **T-0014 bitte über die Inbox am PC beantworten** (Mission Control) — der Regelkanal-Nachweis beginnt mit diesem DR.

## Budget/Arbeitsweise

0 € erwartet; unverändert nach Playbook/Runbook; Statuswechsel via Skript-Route.
