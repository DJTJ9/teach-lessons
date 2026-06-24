# Mission

## Why
Beim nächsten ähnlichen Bug (falsches Routing, stille Fehler, konditionelle Setup-Schritte) sofort die Implementierungs-Pattern abrufen können — ohne den Code nochmal durchsuchen zu müssen.

## Success looks like
- CLI-Flag Pattern (`--bot`) selbst in ähnlichen Scripts implementieren können
- Routing-Map Fallbacks bewusst designen (no-op vs. produktionskritisch)
- Setup-Schritte mit mehreren Konsumenten erkennen und nie bedingt machen

## Constraints
- Fokus: Python-Implementierungsdetails, konkreter Code
- Basis: frisch implementiert — kein Grundlagen-Aufbau nötig

## Out of scope
- argparse deep-dive (wir nutzen manuelles argv-Parsing)
- Telegram Bot API allgemein
- Konzeptuelle Patterns ohne Code-Bezug
