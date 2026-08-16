# Software Requirements — P1 "Mission Control 2.0" (extension of platform baseline)

*Extends SWR-001–024 (p0, baseline genesis-v1.0); numbering continues. Components: BCK/FRT (backend/frontend), ORC (orchestrator), TOOL (scripts). Language: English (D011). Status `reviewed` = feasibility (ARCH/DEV context) + verifiability (QM/TEST context) per DoD checklist. v0.1 Sprint 0, T-0002 — G1 pending.*

| ID | Requirement | Trace | Verification | Prio | Status |
|---|---|---|---|---|---|
| SWR-025 | The backend shall discover project repositories under the workspace root (directories containing `tickets/` and `.git`) and serve board, report, and KPI data scoped per project via a project parameter on every read API. | STK-013 | API tests (two temp projects, scoping, discovery) | high | reviewed |
| SWR-026 | The frontend shall provide a project selector; all views shall show data of the selected project, plus a cross-project overview listing each project's open tickets and open decision requests. | STK-013 | UI acceptance checklist + API tests (overview endpoint) | high | reviewed |
| SWR-027 | The decision inbox shall list open decision requests of all discovered projects and accept decisions per project, writing to the respective project's decision log and ticket with the established validation (options, git commit). | STK-013 | API tests (two projects, decide round-trip, wrong-project rejection) | high | reviewed |
| SWR-028 | The orchestrator tick shall operate on any discovered project via `--projekt`, keeping the existing single-project behavior and validations unchanged for the default case. | STK-013 | Unit tests (project selection, unchanged default) | medium | reviewed |
| SWR-029 | Preflight and traceability tooling shall cover all discovered projects and configured products in one invocation, reporting findings per project/product. | STK-013 | Unit tests (multi-root run) + real run evidence | medium | reviewed |

## Views and notification (Sprint 2, T-0011 — v1.1)

| ID | Requirement | Trace | Verification | Prio | Status |
|---|---|---|---|---|---|
| SWR-030 | The backend shall serve the requirements documents of a project (stakeholder and software markdown files) read-only via API, and the frontend shall render them in a requirements view. | STK-013 | API tests (files served, unknown project 404) + UI check | high | reviewed |
| SWR-031 | The backend shall serve the verification reports of a project (`verification/reports/*.md`, incl. traceability matrices) read-only via API, and the frontend shall render them in a traceability view. | STK-013 | API tests (reports listed/served) + UI check | high | reviewed |
| SWR-032 | The backend shall list the baselines of every repository under the workspace root (annotated git tags with messages) via API, and the frontend shall render them in a baselines view. | STK-013 | API tests (tags listed per repo) + UI check | medium | reviewed |
| SWR-033 | The platform shall send one e-mail notification per new decision request (across all projects) containing project, ID, title and deadline; sent DRs are marked on the ticket, delivery failures are logged and retried on the next run without blocking anything. | STK-013, STK-007 (D004) | Unit tests (marker set only on success, no duplicate send) | high | reviewed |

## Nachtrag v1.2 (pm/N-0019, pm/T-0019, PM-Beschluss B028)

*Betriebs-CR: die Requirements-Ansicht (SWR-030) zeigte ausschließlich das im Kopfbereich gewählte Projekt. Bei 13 Projekten/Teams und 22 Requirements-Dokumenten heißt das: wer nicht weiß, in welchem Repo eine Anforderung liegt, findet sie nicht. Keine neue Projekt-Baseline — `p1-v1.0` bleibt Abnahmereferenz.*

| ID | Requirement | Trace | Verification | Prio | Status |
|---|---|---|---|---|---|
| SWR-085 | The requirements API shall accept the collective value `alle` in place of a single project and then serve the requirements documents of **all** discovered projects and teams in one response, each file carrying its project and that project's cockpit group; the requirements view shall show all documents by default and offer filtering by project/team, by group and by full text, stating how many of how many documents are shown. Scoped single-project queries (SWR-030) shall keep their previous behaviour, including the 404 for unknown projects. | STK-013 | Unit tests (collective query spans all projects, origin present per file, single-project query unchanged, unknown project still rejected) + UI checklist (filters narrow the list, counter matches) | high | reviewed |

## Traceability

STK-013 ← SWR-025–033, SWR-085 (complete; no orphans). DoD checklist applied per SWR (v1.0: 2026-08-07 RM; v1.1 additions SWR-030–033: 2026-08-07 RM — feasibility ARCH/DEV context, verifiability QM/TEST context). G1 v1.1 pending. v1.2: +SWR-085 (Betriebs-CR pm/T-0019 aus pm/N-0019, PM-Beschluss B028).
