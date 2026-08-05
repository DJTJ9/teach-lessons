# Mission

## Why
Den Desk-Buddy Overlay-Spike (Unity 6 + Win32) so tief verstehen, dass ich jede Zeile
des Codes einer anderen Person am Whiteboard erklären kann — und die Overlay-Schicht
selbst in einem neuen Projekt aufsetzen kann, ohne den Spike zu kopieren.

## Success looks like
- Ich kann erklären, **warum** D3D12/Flip-Model Fenster-Transparenz unmöglich macht und
  welche Player Settings daraus zwingend folgen.
- Ich kann `Win32Interop.cs` Zeile für Zeile vorlesen und jeden `DllImport`, jede
  Konstante und jedes `StructLayout` begründen.
- Ich kann die Input-Falle (`Input.mousePosition` friert unter `WS_EX_TRANSPARENT` ein)
  aus dem Kopf erklären und zeigen, warum `GetCursorPos` + Koordinaten-Flip nötig sind.
- Ich kann den Click-through-Zustandsautomaten inkl. DragLock aufmalen und sagen,
  welcher Bug ohne ihn entsteht.
- Ich kann in einem neuen Unity-Projekt ein transparentes, click-through-fähiges
  Overlay-Fenster von Null aufsetzen und weiß, welche Datei ein macOS-Port ersetzt.

## Constraints
- Vorwissen: C# und Unity sehr gut. **Win32 / P/Invoke komplett neu** — jede native
  API, jedes Handle, jede Bitmaske wird von Null erklärt.
- Referenzcode: `github.com/DJTJ9/desk-buddy` (Stand `a57f9f1`, 2026-08-04).
- Transparenz ist im Unity-Editor prinzipiell nicht testbar — jeder Sichttest braucht
  einen Build. Lektionen berücksichtigen das.

## Out of scope
- Prozess-/Workflow-Themen: Spike-Schnitt, Editor-Scripts statt GUI, Batchmode-Build,
  TDD-Vorgehen, 9-Punkte-Beweis-Durchlauf (bewusst abgewählt).
- Alles nach dem Spike: Figur, Animator, Haltungs-Zustandsmaschine, Übungssystem,
  Progression.
- DPI-Scaling, Multi-Monitor, Autostart, Tray-Icon, Installer.
