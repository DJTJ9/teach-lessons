# Mission

## Why
Das gerade gebaute UI-Redesign (Command-Center-Startseite, gebündelte `/onboarding`-Seite, `.safe-sheet`-Panel-Fix, `.hinweis`-Vereinheitlichung) so verstanden haben, dass Tjark es in 5 Minuten einer neuen Kommilitonin erklären kann und beim nächsten Feature auf denselben Mustern aufbaut statt sie neu zu erfinden.

## Success looks like
- Kann erklären, warum die alten 3 Hero-Buttons durch ein Erstbesuch-Banner + 4 Command-Center-Karten ersetzt wurden (und für wen welcher Zustand greift).
- Kann erklären, warum die 4 Onboarding-Popups zu einer Route gebündelt wurden statt 4 Modals zu bleiben.
- Kann das `.safe-sheet`-Muster (sticky Close-Button vor scrollbarem Body) auf ein zukünftiges Fixed-Position-Panel übertragen, ohne den Bug (Close-Button scrollt weg) zu wiederholen.
- Kann benennen, wo Command-Center-Kontext (`primary_profile`, `new_matches`) herkommt und warum er absichtlich nicht in andere Templates weitergereicht wird.

## Constraints
- Kurz — Feature ist bereits live, kein Deep-Dive in FastAPI/Jinja von Grund auf nötig, nur die Entscheidungen dieses Redesigns.
- Tjark kennt die Codebase bereits (Owner), Lektionen sind Konsolidierung/Referenz, kein Einstieg.

## Out of scope
- FastAPI-Grundlagen, Jinja2-Syntax-Einführung — bereits bekannt.
- Die unveränderte Profil-Liste / Wizard-Flow — nicht Teil dieses Redesigns.
