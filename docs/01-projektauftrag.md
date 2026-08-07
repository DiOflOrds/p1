# Projektauftrag P1 — „Mission Control 2.0"

*Version 0.1, 2026-08-07. Erstes Regelprojekt nach P0-Abschluss (D024), gewählt per Intake-DR (D025, Option A). Zur G0-Freigabe durch den Auftraggeber.*

## 1. Ziel

Die eigene Plattform wird vom Bootstrap-Werkzeug zum belastbaren Mehrprojekt-Leitstand ausgebaut — requirements-first, mit denselben Prozessen, die in P0 nachgewiesen wurden. P1 schließt zugleich die drei dokumentierten Abnahme-Reste aus P0 (Kriterien 4/5/9-Abweichungen).

## 2. Scope (Epics, aus dem priorisierten P0-Backlog)

| Epic | Inhalt | Quelle |
|---|---|---|
| P1-E1 | **Multi-Projekt:** Board/Backend/Tick aggregieren und bedienen mehrere Projekt-Repos (p0, p1, künftige); Projektwahl in Mission Control | B1, F8/D023 |
| P1-E2 | **Frontend-Views:** Requirements-Browser, Traceability-Matrix und Baseline-Übersicht als lesende Ansichten | B6, P0-Kriterium 5 |
| P1-E3 | **Inbox als Regelkanal:** alle DRs über die Decision-Inbox, E-Mail-Benachrichtigung real in Betrieb (SMTP-Zugang nötig, DR an Mensch) | B5, P0-Kriterium 4, D004 |
| P1-E4 | **Review-Unabhängigkeit:** definierte externe Stichproben (Mensch oder Zweitsession) je Sprint + Doku im Report | B2, Self-Check |
| P1-E5 | Betriebsreste: Copilot-PoC-Abschluss (T-0072), erster Claude-API-Tick mit Kostendaten (B9/T-0008, optional nach Budgetfreigabe) | B9, Kriterium 9 |

**Nicht im Scope:** neue Produkte, Embedded/SYS-Ausbau (F6-Backlog), VM (D017-Wiedervorlage erst nach P1), MCP-Verpackung (P3).

## 3. Abnahmekriterien (G3 für P1)

1. Zwei Projekte (p0 abgeschlossen, p1 aktiv) sind in einer Mission-Control-Instanz sichtbar und bedienbar.
2. Requirements/Traceability/Baselines sind ohne Git-Zugriff im Frontend einsehbar (P0-Kriterium 5 voll).
3. Mindestens 5 echte DRs liefen in P1 über die Inbox inkl. E-Mail-Benachrichtigung (P0-Kriterium 4 voll).
4. Je Sprint mindestens eine dokumentierte externe Review-Stichprobe.
5. Alle Plattform-Änderungen requirements-first (SWR-Erweiterungen mit G1) und CI-grün; Kriterium 9 voll (Copilot-Lauf protokolliert).

## 4. Rahmen

Nutzer: zunächst Auftraggeber, Ausbau für weitere Personen vorbereitet (F9/D025 — Rechtefragen als Backlog). Vertraulichkeit: alles privat (F10). Budget: Testphasen-Mechanik unverändert (20 €/Monat hart, D012); erwartete API-Kosten 0 € bis T-0008-Freigabe. Betrieb lokal auf Team-Node-1 (D017). Sprache: D011. Gates: G0 (dieser Auftrag), G1 je SWR-Erweiterung, G2 bei Architekturänderungen, G3 (Abnahme), G4 je Sprint.

## 5. Grobplan

Sprint 0 (kurz): Auftrag/G0, Backlog-Detaillierung, SWR-Erweiterungsentwurf Multi-Projekt. Sprint 1: P1-E1 (Multi-Projekt-Kern). Sprint 2: P1-E2 + P1-E3. Sprint 3: P1-E4/E5, Härtung, G3. Re-Planung durch PL transparent erlaubt (Playbook).

## 6. Entscheidung (G0)

**Frage:** Projektauftrag P1 freigeben? Optionen: **G0a** freigeben (Empfehlung) / **G0b** mit Änderungen / **G0c** zurückstellen.
