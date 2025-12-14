
# HWiNFO64 Overlay

A Python code overlay base on HWiNFO64. Display CPU, GPU, RAM, FPS information. Open source & free.

## Features
- CPU/GPU usage, temps, clocks, fan RPM, RAM usage
- FPS from HWiNFO shared memory (when enabled)
- Drag to reposition; stays on top of fullscreen apps
- Toggle/exit via hotkeys and system tray

## Releases (download EXE)
- Download the latest Windows executable from the Releases page: `https://github.com/c47-dev/hwinfo-overlay/releases`.
- Prerequisite: install HWiNFO64 and enable **Shared Memory Support**  
  Download: https://www.hwinfo.com/download/
- Run the EXE; no install needed.

## Requirements
- Windows
- Python 3.9+ recommended
- HWiNFO64 (for shared memory sensors/FPS) with “Shared Memory Support” enabled

Python deps: `PyQt6`, `psutil`, `wmi`, `pywin32`, `keyboard` (@requirements.txt)

Install:
```bash
pip install -r requirements.txt
```

## Config (config.json)
- `position_x`/`position_y`: starting overlay position (pixels)
- `update_interval`: refresh in ms
- `background_opacity`: 0–1
- `background_color`: `R, G, B` string
- `text_color`: label color
- `toggle_hotkey` / `exit_hotkey`: global hotkeys
- `show_full_device_names`: true to show full CPU/GPU names, false for generic

## Running
- Double-click run_overlay.bat (Run as Administrator recommended), or `python main.py`

## Controls
- F12: toggle overlay (default)
- Ctrl+Shift+Q: exit (default)
- Drag with mouse: move overlay