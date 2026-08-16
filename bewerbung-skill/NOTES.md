# Notes

## Lernpräferenzen
- Erstlauf-geführt: jede Lesson hat einen Do-it-Task am echten Repo-Stand.
- Volle technische Tiefe inkl. render.py / Jinja2 / Chrome-Flags — der User hat den Skill selbst gebaut und will Fehler selbst fixen.

## Repo-Stand bei Lesson-Erstellung (2026-08-16)
- `/root/projekte/bewerbung`
- `profil/master.md` — alle Inhaltsfelder `TODO`, Struktur steht
- `profil/portfolio.md` — 3 Slots, alle `TODO`
- `templates/` — cv.html.j2 + cv.css, anschreiben.html.j2 + anschreiben.css, fonts lokal (offline-fähig)
- `scripts/render.py` (92 Zeilen), `scripts/test_render.py` (pytest-Smoke, self-contained Fixture)
- `out/cv-de.pdf`, `out/cv-en.pdf` vorhanden (Probe-Render)
- **kein** `bewerbungen/`-Ordner → Lesson 6–8 legen den ersten an

## Nicht-offensichtliche Fakten, die in die Lessons müssen
- `cv.css`: `body { height: 296mm; overflow: hidden }` → CV ist **hart einseitig**. Zuviel Inhalt wird stillschweigend abgeschnitten, kein Fehler.
- `tr()` greift nur, wenn der Wert ein dict mit Key `de` oder `en` ist; sonst wird der Wert unverändert durchgereicht. Fehlt `en`, fällt es still auf `de` zurück.
- `autoescape=True` → HTML im Markdown-Text wird escaped, nicht gerendert.
- `paragraphs()` splittet am Leerzeile-Regex → jede Leerzeile im Anschreiben-Body = neuer `<p>`.
- Anschreiben-Sprache kommt aus dem Frontmatter (`lang:`), **nicht** aus einem CLI-Flag.
- Default-Output Anschreiben: `<ordner der md-datei>/out/anschreiben-<lang>.pdf`.
