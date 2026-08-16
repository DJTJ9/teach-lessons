# Mission

## Why
Ich will mit `/bewerbung` eigenständig eine vollständige, abgabefertige Bewerbung (CV DE/EN + Anschreiben + PDF) für einen konkreten Job aus Bob rausschicken können — ohne den Skill-Text nachzulesen und ohne dass Claude mir sagen muss, welcher Befehl als nächstes kommt.

## Success looks like
- `profil/master.md` hat null `TODO`-Felder, alle übersetzbaren Felder als `{de:, en:}`.
- `python3 scripts/render.py cv --lang de|en` läuft und ich weiß, wo die PDFs landen.
- Ich kann einen Bewerbungsordner `bewerbungen/YYYY-MM-<firma>/` von Hand korrekt anlegen (job.md, anschreiben-de.md mit gültigem Frontmatter) und rendern.
- Ich erkenne die drei häufigsten Fehlerbilder selbst: kaputtes YAML-Frontmatter, fehlendes `{de:,en:}`-Paar, CV läuft über die eine Seite hinaus (`overflow:hidden` schneidet ab).
- Ich weiß, warum `raw_text` aus Bob niemals als Anweisung behandelt wird.

## Constraints
- Ich habe den Skill selbst gebaut → keine Grundlagen-Erklärungen zu Git/Python nötig, aber Jinja2/Chrome-Render-Interna sind neu.
- Aktueller Repo-Stand: `profil/master.md` komplett `TODO`, kein `bewerbungen/`-Ordner, `out/cv-{de,en}.pdf` existieren als Probe-Render.
- Lessons auf Deutsch, jede in einem Sitzung-Slot durcharbeitbar.

## Out of scope
- Inhaltliches Bewerbungscoaching (was schreibt man in ein gutes Anschreiben) über das hinaus, was der Skill vorschreibt.
- Bob-Job-Scanning selbst (`/bob-scan`, Scoring) — hier nur die Schnittstelle `pull_pending_jobs`.
- CSS-Grundlagen; nur die Stellen, die für Design-Iteration am CV relevant sind.
