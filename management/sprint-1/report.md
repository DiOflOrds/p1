# Sprint-1-Report — P1 „Mission Control 2.0" (PL)

*2026-08-07. Sprint-Motto: „Multi-Projekt-Kern" (P1-E1). An: Mensch (G4-Review). 6/6 Tickets done.*

## Sprint-Ziel: erreicht

Mission Control bedient mehrere Projekte aus einer Instanz: Projekt-Discovery per Konvention (ADR-004, **G2/D002**), gescopte Board/Report/KPI-APIs mit `?projekt=`, neue Standard-Ansicht **Übersicht** (je Projekt offene Tickets + Entscheidungen), projektübergreifende Inbox mit Entscheidung ins jeweilige Projekt, Tick-Projektvalidierung, Preflight-Board-Check und Matrix über alle Projekte/Quellen.

| Ticket | Ergebnis |
|---|---|
| T-0004 | Architektur v1.1 + ADR-004 (Discovery statt Registry) — G2/D002 |
| T-0005 | Backend: Discovery, Scoping, `/api/projekte` + `/api/uebersicht` (SWR-025) |
| T-0006 | Frontend: Projektwahl, Übersicht als Startansicht, projektbewusste Inbox (SWR-026) |
| T-0007 | Inbox über alle Projekte, Entscheidung je Projekt mit voller Validierung (SWR-027) |
| T-0008 | Tick/Preflight/Matrix multi-projektfähig, CI auf zwei SWR-Quellen (SWR-028/029) |
| T-0009 | +9 Tests (Suite **121** grün), Merged-Matrix **29 SWRs / 0 Lücken**, real p0+p1 im Preflight |

## KPIs

Tests 112 → **121** + 42 (produkt) · Matrix 29/0 · 0,00 € API · Statuswechsel 100 % über Skript-Route · Entscheidungen: P1-D002 (G2).

## QM-Abschnitt (ungefiltert)

1. UI-Änderungen (T-0006) sind API-seitig testgedeckt; die Geräte-Abnahme (Selector/Übersicht am Handy/PC) steht aus → bitte beim G4 kurz ansehen. 2. platform-CI wird erst grün, wenn die Lese-PAT um p1 erweitert ist (T-0008-Rest, Anleitung unten). 3. Reviews weiterhin Rollen-Kontexte; **erste externe Stichprobe (P1-E4) = Teil dieses G4.**

## Entscheidungsbedarf an dich (G4)

Abnahme der 6 Tickets. **Bitte als externe Stichprobe (P1-E4) ein Artefakt deiner Wahl selbst prüfen** — Vorschlag: Mission Control starten (`python platform\backend\server.py --repos .` → http://127.0.0.1:8080), Projekt-Selector p0↔p1 durchklicken und die Übersicht ansehen. Optionen: abnehmen / mit Auflagen / zurückweisen.
