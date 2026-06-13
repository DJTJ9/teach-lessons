# Mission

## Why
Run the Telegram-Notion-Bot dauerhaft auf einem Raspberry Pi 4 — ohne offenes Terminal auf dem Windows-Rechner. Bot startet automatisch beim Booten, läuft 24/7, überlebt Neustarts.

## Success looks like
- Raspberry Pi läuft mit Raspberry Pi OS, SSH-Zugang vom PC funktioniert
- Bot-Code liegt auf dem Pi, alle Secrets/Env-Vars sicher konfiguriert
- Bot läuft als systemd-Service (autostart, auto-restart bei Fehler)
- Logs sind lesbar via `journalctl`
- Grundlegende Sicherheit: Firewall aktiv, SSH per Key statt Passwort

## Constraints
- Anfänger in Linux/Server (kaum Terminal-Erfahrung)
- Hardware: Raspberry Pi 4 (4 GB oder 8 GB RAM) — vorhanden, aber noch nicht 24/7 aktiv
- Keine Eile — gründliches Lernen bevorzugt
- Kein öffentlicher Zugriff nötig: Bot kommuniziert nur ausgehend mit Telegram/Notion-API

## Out of scope
- Echter VPS (gemieteter Cloud-Server) — Pi als Home-Server reicht
- Domain, SSL/TLS, reverse Proxy (Nginx) — Bot braucht keinen eingehenden Traffic
- Docker/Container — zu viel Overhead für Anfänger
- Mehrere Services gleichzeitig hosten
