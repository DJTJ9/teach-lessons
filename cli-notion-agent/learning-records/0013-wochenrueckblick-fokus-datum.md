# LR-0013: Wochenrückblick, Fokusblock, Datum-Verschieben

Drei neue Bot-Befehle via System-Prompt-Muster: `woche` (7-Tage-Rückblick), `fokus: Bereich` (heutige Tasks nach Bereich), `verschieben: Datum` (alle offenen Tasks auf neues Datum setzen). Alle nutzen `run_claude()` mit dediziertem System-Prompt — kein eigener Notion-API-Code nötig.
