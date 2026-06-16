# Mission

## Why
Einen Hetzner VPS aufsetzen, um von überall — PC und Android-Handy via Termux — identisch an Web- und Android-App-Projekten mit Claude Code zu arbeiten.

## Success looks like
- SSH-Verbindung vom Handy (`ssh dev`) funktioniert
- Claude Code startet auf dem Server mit Claude Pro Abo
- Android SDK + Node.js für Builds vorhanden
- Tailscale sichert den Zugriff ohne offene Ports

## Constraints
- Budget: ~€10/Monat (Hetzner CX33)
- Gerät: Android-Handy + Windows-PC
- Kein separater API Key — Claude Pro Abo wird genutzt

## Out of scope
- Unity/s&box Spieleentwicklung (GUI-abhängig, kein VPS geeignet)
- CI/CD Pipelines
- Docker/Container-Setup
