# Board (generiert von platform/scripts/board.py — nicht von Hand editieren)

Stand: 2026-08-20 · Tickets: 22


## done (21)

| ID | Titel | Typ | Takt | Rolle | Verantwortlich | Prio | Sprint | blockiert durch |
|---|---|---|---|---|---|---|---|---|
| [T-0001](tickets/T-0001.md) | Epics P1-E1–E5 zu priorisiertem Backlog detaillieren | task | einmalig | pl | Team | hoch | 0 | — |
| [T-0002](tickets/T-0002.md) | SWE.1: SWR-Erweiterung Multi-Projekt (STK-013, SWR-025 ff.) draft → reviewed → G1-Vorlage | task | einmalig | rm | Team | hoch | 0 | — |
| [T-0004](tickets/T-0004.md) | SWE.2: Architektur-Delta Multi-Projekt + ADR-004 → G2 | task | einmalig | arch | Team | hoch | 1 | — |
| [T-0005](tickets/T-0005.md) | Backend: Projekt-Discovery + gescopte Board/Report/KPI-APIs + Übersicht (SWR-025) | task | einmalig | dev | Team | hoch | 1 | T-0004 |
| [T-0006](tickets/T-0006.md) | Frontend: Projektwahl + projektübergreifende Gesamtsicht (SWR-026) | task | einmalig | dev | Team | hoch | 1 | T-0005 |
| [T-0007](tickets/T-0007.md) | Inbox projektübergreifend: listen über alle Projekte, entscheiden je Projekt (SWR-027) | task | einmalig | dev | Team | hoch | 1 | T-0005 |
| [T-0009](tickets/T-0009.md) | SWE.4: Verifikation SWR-025–029, Matrix ohne Lücken, Sprint-Report → G4 | task | einmalig | test | Team | hoch | 1 | T-0005, T-0006, T-0007, T-0008 |
| [T-0011](tickets/T-0011.md) | SWE.1: SWR-030–033 (Views + DR-Benachrichtigung) draft → reviewed → G1 | task | einmalig | rm | Team | hoch | 2 | — |
| [T-0012](tickets/T-0012.md) | Views: Requirements/Traceability/Baselines — API + Frontend (SWR-030–032) | task | einmalig | dev | Team | hoch | 2 | T-0011 |
| [T-0013](tickets/T-0013.md) | DR-Benachrichtigung: Skript dr_benachrichtigung.py — einmalig je DR, ausfalltolerant (SWR-033) | task | einmalig | dev | Team | hoch | 2 | T-0011 |
| [T-0014](tickets/T-0014.md) | DR: SMTP-Zugang für E-Mail-Benachrichtigung einrichten (D004) | decision-request | einmalig | pl | Team | hoch | 2 | — |
| [T-0015](tickets/T-0015.md) | SWE.4: Verifikation SWR-030–033 + Matrix + Sprint-Report → G4 | task | einmalig | test | Team | hoch | 2 | T-0012, T-0013 |
| [T-0017](tickets/T-0017.md) | SMTP aktivieren (D006/S1) + erste echte DR-Mail als Nachweis | task | einmalig | mensch | Team | hoch | 3 | — |
| [T-0020](tickets/T-0020.md) | DR: G3 — Abnahme P1 gegen die Projektauftrag-Kriterien 1–5 | decision-request | einmalig | pl | Team | hoch | 3 | — |
| [T-0022](tickets/T-0022.md) | DR: G4 Sprint 3 + formaler P1-Abschluss (Baseline p1-v1.0) | decision-request | einmalig | pl | Team | hoch | 3 | — |
| [T-0003](tickets/T-0003.md) | P1-Registrierung: board-check-Workflow, BOARD-Grundgerüst, Preflight-/Statusintegration | task | einmalig | cm | Team | mittel | 0 | — |
| [T-0008](tickets/T-0008.md) | Tick-Projektvalidierung + Preflight-Board-Check/Matrix über alle Projekte (SWR-028/029) | task | einmalig | dev | Team | mittel | 1 | T-0004 |
| [T-0010](tickets/T-0010.md) | Prozess-CR (Retro S1): trace_matrix --alle-projekte — SWR-Quellen per Discovery | change-request | einmalig | dev | Team | mittel | 2 | — |
| [T-0019](tickets/T-0019.md) | Geräte-Stichproben dokumentieren (D003 + D005): Selector, Übersicht, neue Tabs | task | einmalig | mensch | Team | mittel | 3 | — |
| [T-0021](tickets/T-0021.md) | Sprint-3-Report + Schluss-Retro → G4 als Inbox-DR | task | einmalig | pl | Team | mittel | 3 | T-0020 |
| [T-0016](tickets/T-0016.md) | Prozess-CR (Retro S2): Stichproben-Zeile in G4-Vorlagen + Zähler im Report | change-request | einmalig | coach | Team | niedrig | 3 | — |

## rejected (1)

| ID | Titel | Typ | Takt | Rolle | Verantwortlich | Prio | Sprint | blockiert durch |
|---|---|---|---|---|---|---|---|---|
| [T-0018](tickets/T-0018.md) | Copilot-PoC-Lauf am Team-Node (p0/T-0072) — P0-Kriterium 9 vervollständigen | task | einmalig | mensch | Team | mittel | 3 | — |
