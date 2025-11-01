PrecisionCut Releases
# PrecisionCut

Fast DXF/SVG → G‑code for CNC (GRBL, LinuxCNC, Mach3, Fanuc). Windows installer included.

## Download
- Latest release: https://github.com/jatindersse/PrecisionCut/releases
- Download “PrecisionCut-Setup-<version>.exe” and run it (no admin required).

## Install & Run
1) Double‑click the installer.
2) Launch: Start Menu → PrecisionCut (or `%LOCALAPPDATA%\Programs\PrecisionCut\PrecisionCut.exe`).
3) First run: click “Browse”, select your `.dxf`/`.svg`, set Material/Quality/Post, then “Convert to G‑Code”.
4) When prompted, choose where to save the `.nc` file (any folder you like).
5) Optional: “Send to Machine” (Serial/FTP) or “Open NC Viewer”.

## Update
- In app: click “Check for Updates” → Download → “Install now”.
- If it doesn’t relaunch, the installer log is at `%TEMP%\PrecisionCut-Installer-<version>.log`.

## Troubleshooting
- “Unauthorized changes blocked” or “G‑Code file not found”:
  - Windows Controlled Folder Access is blocking writes. Either allow `PrecisionCut.exe` in
    Windows Security → Ransomware protection → Allowed apps, or save the `.nc` to a different folder when prompted.
- SmartScreen: click “More info” → “Run anyway”.

## Requirements
- Windows 10/11 x64
- USB serial driver (for GRBL/FluidNC, if sending via serial)

git add README.md
git commit -m "Docs: add release download, install, update and troubleshooting"
git push
