# Tasks
 
A personal task management app for the things that are easy to lose track of over time — hobbies, study directions, recurring maintenance, personal commitments, and long-running projects without loud external deadlines.
 
Local-first, SQLite-backed, available on macOS, Windows, and Linux.
 
---
 
## Download
 
Go to the [Releases](https://github.com/mnougerede/tasks-releases/releases/latest) page and download the file for your platform:
 
| Platform | File |
|---|---|
| macOS (Apple Silicon / Intel) | `.dmg` |
| Windows | `.exe` (NSIS installer) |
| Linux (Debian/Ubuntu) | `.deb` |
| Linux (other distros, x64 / arm64) | `.AppImage` |
 
---
 
## Installation
 
### macOS
 
1. Download the `.dmg` file.
2. Open it and drag **Tasks** into your Applications folder.
3. On first launch, right-click the app and choose **Open** to bypass Gatekeeper if needed.
 
### Windows
 
1. Download the `.exe` installer.
2. Run it and follow the prompts.
 
### Linux — one-liner (recommended)
 
```bash
curl -sSL https://github.com/mnougerede/tasks-releases/releases/latest/download/install-linux.sh | bash
```
 
This script auto-detects your architecture (x64 / arm64) and installs a `.deb` package on Debian/Ubuntu systems, or an AppImage with a desktop entry everywhere else.
 
**Requirements:** `curl` and `jq` must be installed.
 
### Linux — manual
 
Download the `.deb` or `.AppImage` directly from the [Releases](https://github.com/mnougerede/tasks-releases/releases/latest) page.
 
**AppImage:**
```bash
chmod +x Tasks-*.AppImage
./Tasks-*.AppImage
```
 
**.deb (Debian/Ubuntu):**
```bash
sudo dpkg -i tasks-*.deb
```
 
---
 
## Data
 
Your data is stored locally in a SQLite file:
 
- **macOS:** `~/Library/Application Support/Tasks/tasks.sqlite`
- **Windows:** `%APPDATA%\Tasks\tasks.sqlite`
- **Linux:** `~/.config/Tasks/tasks.sqlite`
 
The app does not send data anywhere. Backups are written automatically alongside the main database file.
 
---
 
## Source
 
This repository contains release artifacts only. The source code lives at [mnougerede/task-management-app](https://github.com/mnougerede/task-management-app).
 
This repository contains release artifacts only.
