# Mission

## Why
Voice Flow (lokaler Wispr-Flow-Klon) auf einem zweiten Windows-Gerät (Laptop) selbstständig
installieren und starten können, ohne bei jedem Schritt nachzufragen — inklusive der Fehler,
die beim ersten Laptop-Setup tatsächlich aufgetreten sind (Execution Policy, CUDA-DLL,
Claude-CLI-Login).

## Success looks like
- Auf einem frischen Windows-Rechner: Python 3.12, Git, Node/Claude-CLI installiert
- Repo geklont, venv gebaut, Dependencies installiert (inkl. optionaler GPU-Pakete)
- `claude` CLI eingeloggt
- App startet via `start.bat` / `start_silent.vbs`, Hotkey diktiert Text korrekt
- Bei den drei bekannten Fehlerbildern (PowerShell Execution Policy, cublas-DLL fehlt,
  401 Invalid authentication) selbst erkennen, was los ist, und den Fix anwenden

## Constraints
- Nur Windows (App-Code ist aktuell Windows-only: `paste_windows.py`, `hotkey_windows.py`)
- Bilder sind nachgebaute SVG-Mockups der echten Dialoge, keine echten Screenshots
  (kein Bildschirmzugriff auf das Zielgerät)
- Repo ist privat auf GitHub (`DJTJ9/voice-recorder`) — Guide geht von Lesezugriff aus

## Out of scope
- Mac/Linux-Installation (App-Code unterstützt das aktuell nicht, bräuchte Portierung)
- iPad/Android-Setup (andere Architektur, siehe Voice-Flow-Roadmap)
- GPU-Treiber-Installation im Detail (nur Kurzhinweis, NVIDIA-Support-Seiten sind autoritativ)
