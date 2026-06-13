# Mission

## Why
TDD ist in vielen Jobbeschreibungen als Grundvoraussetzung gelistet. Ziel: selbstständig neue Features test-first entwickeln können — nicht erst Code schreiben, dann Tests hinzufügen.

## Success looks like
- Red-Green-Refactor Zyklus auswendig anwenden
- Tests für den Telegram-Chatbot mit pytest schreiben (test-first, nicht post-hoc)
- Unity-Tests mit NUnit schreiben für Spielemechaniken
- Testtypen korrekt unterscheiden (Unit / Integration / E2E)
- Test-Smells erkennen und vermeiden
- Mocking/Patching für externe Abhängigkeiten (Telegram API, Notion API) nutzen

## Constraints
- Bekannte Sprachen: Python (pytest vorhanden, aber post-hoc), C# (Unity)
- 6+ Stunden pro Woche
- Praxisbeispiele: `bot.py` Chatbot + Unity/C#
- Vorhandene Tests in `tests/` als Ausgangspunkt

## Out of scope
- E2E-Testing mit Selenium/Playwright
- CI/CD Pipelines
- Performance-Testing
- pytest-Plugins jenseits von monkeypatch/tmp_path
