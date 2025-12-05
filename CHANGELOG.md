# Changelog

## [0.4.0] - 2025-12-05

![Recording](images/v0.4.0/recording.png)

### Transcription is Now Lightning Fast
- Record as long as you want - transcription happens in the background
- No more waiting after you stop recording
- GPU-accelerated processing (70% faster)
- Silence trimming for cleaner results

### New Features

**Dictation:** Clipboard mode `⌥⇧A`, clipboard stack with hover preview, language/model selection, silence sensitivity

![Dictation History](images/v0.4.0/dictation-history.png)

**Session:** Screen time tracking, sleep detection, idle alerts (15min-2h), lifecycle reset (5-7h sleep breaks)

![Session](images/v0.4.0/session.png)

**Display:** XDR brightness beyond normal limits on supported displays

![Display Menu](images/v0.4.0/display-menu.png)

**Tools:** Keyboard cleaner, hotkey panel, secure API key storage (Keychain), crash reporting (Sentry)

![Tools](images/v0.4.0/tools.png)

![Keyboard Cleaner](images/v0.4.0/keyboard-cleaner-panel.png)

### Better Experience
- UI never freezes anymore - ML runs on dedicated thread
- Hotkeys respond instantly on their own thread
- Permissions requested when needed, not at startup
- Pipeline feedback: REC → Recorded → % → ✓ Pasted
- Stuck hint `(⌥⎋)` appears when transcription hangs for 3+ seconds
- Inline clipboard badges in transcription history
- New app icon

### Menu & Settings

![About](images/v0.4.0/about.png)

- "Check for Updates..." moved to top level (macOS native style)
- Auto-update toggle moved to About panel
- Developer menu hidden in production builds
- About panel with GitHub links (What's New, Report a Problem)

### Fixes
- ESC key works correctly in all contexts
- Arrow keys work when search is focused
- Playback cleanup on manual stop
- Session time persists across restarts

## [0.3.0] - 2025-11-28

### New Features
- Display brightness control (F1/F2)
- Toggle built-in display off
- Transcription history with search

## [0.2.0] - 2025-11-26

### Initial Release
- Voice dictation with WhisperKit
- Global hotkeys
- Menu bar interface
- Auto updates via Sparkle
