# Schluss-Retrospektive P1 — Sprint 3 + Projekt (COACH)

*2026-08-15.*

**Gut über das Projekt:** Drei Sprints, drei Baselines, 12 SWRs requirements-first umgesetzt, alle Gates real (2 davon über die selbst gebaute Inbox); die Discovery-Idee (ADR-004) hat drei Pflege-Mechanismen eliminiert; der Mensch-Anteil sank sichtbar — Sprint 3 bestand teamseitig fast nur noch aus Verbuchen.

**Hakte (ehrlich):** 1. Der E-Mail-Erstbetrieb brauchte drei Anläufe (2FA fehlte → falsches Passwort im alten Fenster → Alt-Adresse) — Erst-Einrichtungen mit externen Diensten verdienen eine Checkliste statt Trial-and-Error. 2. DR-Fristen liefen ab, ohne dass es jemand merkte (Mail-Kanal kam erst danach). 3. Copilot-PoC scheiterte an fehlender CLI-Installation — Geräte-Voraussetzungen standen nur im Ticket, nicht im Geräteregister.

**Empfehlungen ins Backlog (kein neuer Sprint — Projekt endet):** R1 Runbook-Checkliste „externer Dienst einrichten" (2FA/Secrets/Testlauf/Empfänger prüfen); R2 Frist-Warnung im dr_benachrichtigung-Lauf (DRs nahe/über Frist erneut mailen); R3 Geräteregister um Soll-Toolchain je PoC ergänzen (Copilot CLI). Übergabe an den Betrieb bzw. das nächste Projekt.
