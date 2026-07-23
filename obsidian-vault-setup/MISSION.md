# Mission

## Why
Alle eigenen Geräte (Windows-Laptop, iPad, Android-Handy) sollen vollständig mit dem eigenen Obsidian-Vault synchronisiert sein — Notizen und, wo technisch möglich, Web-Clipper-Funktionalität überall verfügbar, genau wie am bestehenden Desktop-Setup.

## Success looks like
- Self-hosted LiveSync auf Windows-Gerät eingerichtet, Vault vollständig übernommen (Fetch statt Rebuild)
- Obsidian-App auf iPad eingerichtet, gleiche LiveSync-Verbindung aktiv
- Obsidian-App auf Android-Handy eingerichtet, gleiche LiveSync-Verbindung aktiv
- Web Clipper dort eingerichtet, wo die Plattform es zulässt (Desktop-Browser); auf iPad/Android dokumentierte Alternative für "Wissen reinspeichern"

## Constraints
- Sync läuft selbst-gehostet über CouchDB (sync.thinkshark.de) + Self-hosted LiveSync Plugin, nicht über offiziellen Obsidian Sync Dienst
- Keine echten Zugangsdaten in den Lesson-Inhalten (Lessons landen öffentlich auf GitHub Pages) — nur Platzhalter + Hinweis, wo die echten Werte zu holen sind
- Kein Web Clipper als Browser-Extension auf iOS/Android möglich (offizielle Extension ist Desktop-Browser-only)

## Out of scope
- Einrichtung des CouchDB-Servers selbst (existiert bereits)
- Tiefe Evaluierung mobiler Clipper-Alternativen — nur kurz dokumentiert
