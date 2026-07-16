# Mission

## Why
Ein Besucher der Job-Scanner-Website (job-scanner.thinkshark.de) — Kommilitonin, Recruiter, technisch interessierter Portfolio-Betrachter — soll nach dem Lesen erklären können, was Job-Scanner ist, welche Technologien es benutzt und wie eine Stellenanzeige vom Scraping bis zur Score-Anzeige im Dashboard verarbeitet wird. Die Lektion ist die Quelle für die Kurzfassung + den Link im Onboarding-Panel "Wer bin ich und was kann ich?" auf der Homepage.

## Success looks like
- Kann in 2-3 Sätzen sagen, was Job-Scanner tut und für wen es gebaut wurde (Portfolio-Projekt, Quereinsteiger-Jobsuche als Ursprung).
- Kann den Tech-Stack benennen (FastAPI/SQLite/Jinja2, Playwright+Firecrawl-CLI+Groq als Scraping-Layer, Claude-Agenten für Scoring/Feedback, systemd-Timer für Automatisierung).
- Kann den Datenfluss in eigenen Worten skizzieren: Portale → Scraping/Dedup → Storage (SQLite) → Scoring nach persönlichen Kriterien → Dashboard → Feedback-Loop passt Gewichte an.

## Constraints
- Ein Lese-Durchgang, keine Vorkenntnisse in FastAPI/SQLite vorausgesetzt — Begriffe kurz erklärt, keine Code-Tiefe.
- Muss als Kurzfassung + Link auf einer bereits designten Website-Panel-Fläche funktionieren (Echolot-Theme, kein neues Design).
- Eine einzige Lektion (User-Entscheidung: "Alles in einer Lektion"), kein mehrteiliger Kurs.

## Out of scope
- Keine Anleitung zum Selbst-Deployen/Forken des Projekts.
- Kein Deep-Dive in einzelne Scoring-Formeln oder SQL-Schemata (nur Konzept-Ebene).
- Keine Bewertung/Vergleich mit anderen Jobbörsen-Tools.
- Keine Owner-vs-Member-Rollenunterscheidung im Text — geplante Weiterentwicklung gleicht Member-Funktionalität an den Owner an, die Lektion soll nicht auf einer Unterscheidung aufbauen, die bald hinfällig wird.
