# Sprint-1-Plan — P1 „Mission Control 2.0" (PL)

*Erstellt 2026-08-07. Sprint-Motto: „Multi-Projekt-Kern" (P1-E1). Basis: `p1-req-v1.0` (G1/D001).*

## Sprint-Ziel

Mission Control bedient mehrere Projekte aus einer Instanz: Projekt-Discovery und gescopte APIs im Backend (SWR-025), Projektwahl + projektübergreifende Übersicht im Frontend (SWR-026), Inbox über alle Projekte (SWR-027), Tick auf beliebigen Projekten (SWR-028), Preflight/Matrix über alles in einem Lauf (SWR-029) — vollständig testgedeckt, Matrix ohne Lücken.

## Sprint-Backlog

| # | Ticket | Inhalt | Rolle | SWR | blocked_by |
|---|---|---|---|---|---|
| 1 | T-0004 | Architektur-Delta Multi-Projekt + ADR-004 → G2 | ARCH | alle | — |
| 2 | T-0005 | Backend: Discovery + gescopte Board/Report/KPI-APIs + Übersicht | DEV | SWR-025 | T-0004 |
| 3 | T-0006 | Frontend: Projektwahl + Gesamtsicht | DEV | SWR-026 | T-0005 |
| 4 | T-0007 | Inbox projektübergreifend (listen + entscheiden je Projekt) | DEV | SWR-027 | T-0005 |
| 5 | T-0008 | Tick-Projektvalidierung; Preflight-Board-Check + Matrix über alle Projekte | DEV | SWR-028/029 | T-0004 |
| 6 | T-0009 | Verifikation: Tests je SWR, Matrix-Erweiterung (p0+p1-SWR-Quellen), Report → G4 | TEST | alle | T-0005–T-0008 |

## Human-Gates

**G2** (Architektur-Delta, T-0004). **G4** (Sprint-Review) — inkl. **erster externer Review-Stichprobe durch dich** (P1-E4: du siehst dir ein Artefakt deiner Wahl an und vermerkst das im Review). Einmalig nötig: bestehende Lese-PAT um das p1-Repo erweitern (für das Matrix-Gate der platform-CI; Anleitung folgt beim Abschluss).

## Budget/Arbeitsweise

0 € erwartet; Statuswechsel via `board.py status`, Commits mit Ticket-ID + SWR-Bezug, requirements-first gegen `p1-req-v1.0`; Preflight je Start (grün gelaufen).
