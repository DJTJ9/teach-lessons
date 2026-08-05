# Notes

## Lernender
- C#/Unity sehr gut → keine MonoBehaviour-/Kamera-/Sprite-Grundlagen erklären.
- Win32/P-Invoke komplett neu → HWND, DllImport, Bitmasken, Structs von Null aufbauen.
- Ziel ist Erklärbarkeit an Dritte **und** Wiederverwendung in neuen Projekten.

## Scope-Entscheidung (2026-08-05)
Nur Overlay-Technik. Prozessthemen (Spike-Schnitt, Editor-Scripts statt GUI,
Batchmode-Build, TDD-Schnitt, 9-Punkte-Beweis) abgewählt.

## Quellenlage
Code-Stand aus `github.com/DJTJ9/desk-buddy` @ `a57f9f1` geklont und gelesen —
Lektionen zitieren den **finalen** Code, nicht den Plan-Entwurf. Zwei Abweichungen
Plan → final: `ClickFeedback.OnMouseOver` mit Rechtsklick-Quit (`7d7a829`),
`IdleProbe` nutzt `Win32Interop.GetWorkingSetBytes()` statt `Process.WorkingSet64`
(`299a7dd`).
