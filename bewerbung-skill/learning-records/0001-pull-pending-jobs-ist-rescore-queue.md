# LR-0001: `pull_pending_jobs` ist die Rescore-Queue, keine Bewerbungsliste

`SKILL.md` (bewerbung) nennt in Schritt 1 von `anschreiben` das Bob-MCP-Tool `pull_pending_jobs` als Job-Quelle "(Favoriten/hoher Score zuerst)". Die Tool-Beschreibung des Servers sagt aber: "Eigene bereits gescorte Jobs, die nach Learn-Insights ein LLM-Rescore brauchen" — also die Warteschlange für `/bob-rescore`. Steht nichts zum Rescoren an, kommt eine leere Liste zurück, obwohl es sehr wohl Bewerbungs-Kandidaten gibt.

Der Weg mit vollem Job-Kontext ist `get_my_votes` (👍/👎 mit Job-Kontext); `get_my_profile.favorites` liefert nur Titel, keine URL. Der robusteste Weg bleibt der eingefügte Anzeigentext.

status: active
evidence: Tool-Beschreibungen via ToolSearch geprüft; `get_my_profile` live aufgerufen — `favorites` enthält ausschließlich `title`.
