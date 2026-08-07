# Software Requirements — P1 "Mission Control 2.0" (extension of platform baseline)

*Extends SWR-001–024 (p0, baseline genesis-v1.0); numbering continues. Components: BCK/FRT (backend/frontend), ORC (orchestrator), TOOL (scripts). Language: English (D011). Status `reviewed` = feasibility (ARCH/DEV context) + verifiability (QM/TEST context) per DoD checklist. v0.1 Sprint 0, T-0002 — G1 pending.*

| ID | Requirement | Trace | Verification | Prio | Status |
|---|---|---|---|---|---|
| SWR-025 | The backend shall discover project repositories under the workspace root (directories containing `tickets/` and `.git`) and serve board, report, and KPI data scoped per project via a project parameter on every read API. | STK-013 | API tests (two temp projects, scoping, discovery) | high | reviewed |
| SWR-026 | The frontend shall provide a project selector; all views shall show data of the selected project, plus a cross-project overview listing each project's open tickets and open decision requests. | STK-013 | UI acceptance checklist + API tests (overview endpoint) | high | reviewed |
| SWR-027 | The decision inbox shall list open decision requests of all discovered projects and accept decisions per project, writing to the respective project's decision log and ticket with the established validation (options, git commit). | STK-013 | API tests (two projects, decide round-trip, wrong-project rejection) | high | reviewed |
| SWR-028 | The orchestrator tick shall operate on any discovered project via `--projekt`, keeping the existing single-project behavior and validations unchanged for the default case. | STK-013 | Unit tests (project selection, unchanged default) | medium | reviewed |
| SWR-029 | Preflight and traceability tooling shall cover all discovered projects and configured products in one invocation, reporting findings per project/product. | STK-013 | Unit tests (multi-root run) + real run evidence | medium | reviewed |

## Traceability

STK-013 ← SWR-025–029 (complete; no orphans). DoD checklist applied per SWR 2026-08-07 (RM; reviews: feasibility ARCH/DEV context — builds on existing repos_im_root/produkte.yaml mechanics; verifiability QM/TEST context).
