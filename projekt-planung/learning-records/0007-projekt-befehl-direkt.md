# LR-0007: projekt: Befehl — direkter Zugriff per Notion-Display-Name

`dart: tasks` hat zwei Jobs: Arbeitsverzeichnis UND Notion-Name — Kopplung, die für reine Notion-Abfragen unnötig ist. Ein dedizierter `projekt: <Name>` Zweig übergibt den Anzeigenamen direkt an PROJEKT_TASKS_SYSTEM_PROMPT, ohne `PROJECTS`-Dict-Lookup. Einfacher, generischer: jeder Notion-Projektname funktioniert — auch Projekte die nicht im Dict stehen.

evidence: Lektion 7 erstellt; Unterschied zwischen code-key-Routing und display-name-Routing verstanden
