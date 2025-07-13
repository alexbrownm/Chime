# Chime
Floresville, TX, USA
# 🔔 ChimeX - Smart CLI Sound Notifications

**ChimeX** is a lightweight, customizable sound notification library for Python. It plays notification sounds on command-line events like success, warning, or error — helping you stay in the loop even when your terminal is minimized.

Inspired by [`chime`](https://github.com/MaxHalford/chime), but with expanded theme support, OS compatibility, and integration hooks for automation tools.

---

## 🚀 Features

- ✅ Simple `chimex.success()` / `chimex.error()` syntax
- 🎵 Multiple sound themes: `mario`, `windows`, `anime`, `custom`
- 🔧 Cross-platform support (macOS, Linux, Windows)
- 🧩 Integration with `subprocess`, `try/except`, shell scripts
- ⏱️ Optional delay, loop, or async playback
- 🧪 Test-friendly (mute or log mode for CI/CD)

---

## 📦 Installation

```bash
pip install chimex


import chimex

chimex.theme('mario')  # Options: 'mario', 'windows', 'anime', 'custom'
chimex.success()       # Plays a "success" sound

try:
    # Your code logic
    result = 1 / 0
except ZeroDivisionError:
    chimex.error()

# Play manually
chimex.warning()
