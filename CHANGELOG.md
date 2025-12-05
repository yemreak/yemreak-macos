# Changelog

## [0.4.0] - 2025-12-05

### Transcription is Now Lightning Fast
- Record as long as you want - transcription happens in the background
- No more waiting after you stop recording
- GPU-accelerated processing (70% faster)
- Silence trimming for cleaner results

### New Features
- **Clipboard Mode** `Option+Shift+A`: Transcription with clipboard context
- **Clipboard Stack**: Visual preview of copied items during recording (hover to expand)
- **Language Selection**: Choose transcription language from menu
- **Model Selection**: Switch between Whisper models (Accurate, Fast)
- **Silence Sensitivity**: Adjust chunk detection sensitivity
- **Session Tracking**: Screen time tracking with sleep detection and idle alerts
- **Idle Reset**: Auto-pause tracking after inactivity (15min to 2 hours)
- **Lifecycle Reset**: Detect sleep breaks (5-7 hours) and start fresh
- **Session Notifications**: Get alerts for session milestones
- **XDR Brightness**: Push brightness beyond normal limits on supported displays
- **Keyboard Cleaner**: Lock keyboard temporarily for safe cleaning
- **Hotkey Panel**: Customize all hotkeys with visual recorder
- **Secure API Key Storage**: Store API keys safely in macOS Keychain
- **Crash Reporting**: Automatic stability monitoring with Sentry

### Better Experience
- UI never freezes anymore - ML runs on dedicated thread
- Hotkeys respond instantly on their own thread
- Permissions requested when needed, not at startup
- Pipeline feedback: REC -> Recorded -> % -> Pasted
- Stuck hint `(Option+Escape)` appears when transcription hangs for 3+ seconds
- Inline clipboard badges in transcription history
- New app icon

### Menu & Settings
- "Check for Updates..." moved to top level (macOS native style)
- Auto-update toggle moved to About panel
- Developer menu hidden in production builds
- About panel with GitHub links (What's New, Report a Problem)

### Fixes
- ESC key works correctly in all contexts
- Arrow keys work when search is focused
- Playback cleanup on manual stop
- Session time persists across restarts

### Screenshots

![Recording](images/v0.4.0/recording.png)
![Dictation History](images/v0.4.0/dictation-history.png)
![Session](images/v0.4.0/session.png)
![Display Menu](images/v0.4.0/display-menu.png)
![Tools](images/v0.4.0/tools.png)
![Keyboard Cleaner](images/v0.4.0/keyboard-cleaner-panel.png)
![About](images/v0.4.0/about.png)

---

## [0.3.0] - 2025-11-28

### New Features
- Display brightness control (F1/F2)
- Toggle built-in display off
- Transcription history with search

---

## [0.2.0] - 2025-11-26

### Initial Release
- Voice dictation with WhisperKit
- Global hotkeys
- Menu bar interface
- Auto updates via Sparkle
