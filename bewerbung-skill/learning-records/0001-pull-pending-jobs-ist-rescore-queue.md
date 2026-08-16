# LR-0001: `pull_pending_jobs` ist die Rescore-Queue, keine Bewerbungsliste

`pull_pending_jobs` liefert laut Bob-MCP-Beschreibung "eigene bereits gescorte Jobs, die nach Learn-Insights ein LLM-Rescore brauchen" — die Warteschlange für `/bob-rescore`. Steht nichts zum Rescoren an, kommt eine leere Liste zurück, obwohl es sehr wohl Bewerbungs-Kandidaten gibt.

Der Weg mit vollem Job-Kontext ist `get_my_votes` (👍/👎 mit Job-Kontext); `get_my_profile.favorites` liefert nur Titel, keine URL. Der robusteste Weg bleibt der eingefügte Anzeigentext.

`SKILL.md` (bewerbung) nannte in Schritt 1 von `anschreiben` ursprünglich `pull_pending_jobs` als Job-Quelle "(Favoriten/hoher Score zuerst)". Am 2026-08-16 korrigiert (Commit `efc1af2` in `/root/.claude`): Schritt 1 nennt jetzt `get_my_votes` und schließt `pull_pending_jobs` ausdrücklich aus.

status: active
evidence: Tool-Beschreibungen via ToolSearch geprüft; `get_my_profile` live aufgerufen — `favorites` enthält ausschließlich `title`. Fix in SKILL.md committet.
