# Resources

## Knowledge
- [Win32 Extended Window Styles (Microsoft Learn)](https://learn.microsoft.com/en-us/windows/win32/winmsg/extended-window-styles) — Nachschlagewerk für `WS_EX_LAYERED`, `WS_EX_TRANSPARENT`, `WS_EX_TOOLWINDOW`.
- [SetWindowLongPtrW (Microsoft Learn)](https://learn.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-setwindowlongptrw) — Fensterstile zur Laufzeit ändern; Erklärung der `GWL_*`-Indizes.
- [SetWindowPos (Microsoft Learn)](https://learn.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-setwindowpos) — Position, Z-Order (`HWND_TOPMOST`), `SWP_*`-Flags.
- [SetLayeredWindowAttributes (Microsoft Learn)](https://learn.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-setlayeredwindowattributes) — Alpha/Colorkey für Layered Windows.
- [DwmExtendFrameIntoClientArea (Microsoft Learn)](https://learn.microsoft.com/en-us/windows/win32/api/dwmapi/nf-dwmapi-dwmextendframeintoclientarea) — der "Glas nach innen ziehen"-Trick mit `MARGINS = -1`.
- [GetProcessMemoryInfo / PROCESS_MEMORY_COUNTERS (Microsoft Learn)](https://learn.microsoft.com/en-us/windows/win32/api/psapi/nf-psapi-getprocessmemoryinfo) — echter Working-Set-Wert, weil Mono `Process.WorkingSet64` still 0 liefert.
- [PlayerSettings.useFlipModelSwapchain (Unity Docs)](https://docs.unity3d.com/ScriptReference/PlayerSettings-useFlipModelSwapchain.html) — die Einstellung, ohne die Transparenz scheitert.
- [Physics2D.OverlapPoint (Unity Docs)](https://docs.unity3d.com/ScriptReference/Physics2D.OverlapPoint.html) — Punkt-Test statt Raycast für 2D-Hit-Test.
- [P/Invoke Marshalling (Microsoft Learn)](https://learn.microsoft.com/en-us/dotnet/framework/interop/marshalling-data-with-platform-invoke) — wie `DllImport`, `StructLayout` und `MarshalAs` zusammenspielen.

## Wisdom (communities)
- [Unity Discussions — transparent + click-through window](https://discussions.unity.com/t/how-to-make-a-unity-game-window-transparent-and-click-through/1704947) — der Thread, in dem die typischen Fehlschläge (schwarze Box, Click-through hängt) diskutiert werden.
- [kirurobo/UniWindowController](https://github.com/kirurobo/UniWindowController) — MIT-Referenzimplementierung (Unity 2022.3); als Lesequelle wertvoll, im Spike bewusst nicht eingebunden.

## Gaps
- Keine belastbare Primärquelle, die "D3D12-Flip-Model + `DwmExtendFrameIntoClientArea`" offiziell als unmöglich dokumentiert — die Aussage stützt sich auf DXGI-Flip-Model-Doku plus übereinstimmende Community-Berichte.
- Keine Quelle zu DPI-Scaling/Multi-Monitor für dieses Fensterkonzept (bewusst out of scope, wird beim Weiterbau gebraucht).
