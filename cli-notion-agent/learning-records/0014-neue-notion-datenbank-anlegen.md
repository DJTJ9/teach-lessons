# LR-0013: Neue Notion-Datenbank per CC Prompt anlegen

Neue DBs brauchen eine `parent_page_id` (Organizer-Seite) und eine `data_source_id` die danach in `CLAUDE.md` gespeichert wird. Properties-Typen: `title`, `status`, `select`, `multi_select`, `rich_text`. `select` für exklusiv-eine-Wahl, `multi_select` wenn mehrere Werte möglich (z.B. Genre). Jede DB bekommt eigenen System-Prompt + Bot-Prefix nach dem `Task:`-Muster aus LR-0012.

evidence: Lektionen 14 und 15 erstellt — Lernthemen-DB (select-Properties) und Spieleideen-DB (multi_select für Genre).
