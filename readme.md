# 🎵 Lyrion Music Server Plugin (Extended)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen)
![Domoticz](https://img.shields.io/badge/Domoticz-2024%2B-blue)
![Python](https://img.shields.io/badge/Python-3.x-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

This plugin provides full integration between **Lyrion Music Server (LMS)** and **Domoticz**.  
The plugin has been fully rewritten, extended, tested, and is stable on Domoticz 2024+.

---
### 🎛️ **Full LMS Remote Control**
- Play / Pause / Stop
- Next / Previous track
- Volume control (dimmer)
- Power On/Off
- Sync / Unsync players

### 📡 **Automatic Player Detection**
- Detects all connected LMS players automatically
- Creates Domoticz devices for each player

### 📊 **Extended Player Information**
- Current track
- Artist
- Album
- Playback status
- Volume
- Online/offline status

### 🎶 **Playlist Support**
- Load playlists per player
- Add tracks to playlist
- Clear playlist
- Start playlists directly via Domoticz or scripts

### 🧠 **Reliable JSON-RPC Communication**
- Full support for `jsonrpc.js`
- Fully tested with Material Skin UI
- Compatible with LMS 8.x

---

## 🛠️ Technical Improvements

- New plugin structure following Domoticz 2024+ standards
- Heartbeat fix (no crashes for missing functions)
- Faster player status parsing
- Reduced API requests → more efficient CPU usage
- Improved error handling + debug logging

---

## 📦 Installation

### Prerequisites

1. Domoticz 2024+ with Python plugin support enabled.
2. Python 3 with the matching Python development package for your system.
3. Install the required Python library:

```bash
sudo apt-get update
sudo apt-get install python3 python3-dev python3-requests
```

Or install the Python dependency with pip:

```bash
python3 -m pip install -r requirements.txt
```

`Domoticz` is provided by Domoticz and is not a pip dependency.

Clone the plugin into the Domoticz plugin folder:

```bash
cd /home/<user>/domoticz/plugins
git clone https://github.com/MadPatrick/domoticz_Lyrion.git lyrion
sudo systemctl restart domoticz

```
