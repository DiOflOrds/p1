# Retrospektive Sprint 1 — P1 (COACH)

*2026-08-07. Regel: max. 3 Verbesserungs-CRs.*

**Gut:** Requirements-first durchgängig (SWR-025–029 vor jeder Codezeile, G1→G2→Implementierung→Verifikation in einem Sprint); Status-Disziplin 100 % über Skript-Route; Merged-Matrix fand sofort die richtige Gesamtzahl (29/0).

**Hakte (ehrlich):** 1. UI-Verifikation nur API-seitig — Geräte-Stichprobe auf nach G4 verschoben (offen, D003). 2. SWR-Quellen der Matrix sind in abschluss.cmd/CI hart kodiert — bei jedem neuen Projekt ein Pflege-Schritt (widerspricht dem ADR-004-Geist). 3. Mensch-Schritt PAT-Erweiterung bremst CI einmalig (kein CR — dokumentiert).

**CR für Sprint 2:** T-0010 — trace_matrix `--alle-projekte`: SWR-Quellen per Discovery (Projekte mit `requirements/software/software-requirements.md`) statt Aufzählung; abschluss.cmd/CI umstellen. Erwartungswert: 0 Pflege-Schritte je neuem Projekt.
