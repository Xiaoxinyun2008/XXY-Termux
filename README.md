# 🚀 XXY - Universal Edition v29.0: The Ultimate Termux Container Manager

<div align="center">

[![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge&logo=termux&logoColor=white)](https://github.com/)
[![Version](https://img.shields.io/badge/Version-v29.0-blue?style=for-the-badge)](https://github.com/)
[![License](https://img.shields.io/badge/License-GPL--3.0-red?style=for-the-badge)](LICENSE)
[![Language](https://img.shields.io/badge/Lang-Bash%20Script-yellow?style=for-the-badge&logo=gnu-bash&logoColor=white)](https://www.gnu.org/software/bash/)

</div>

---

## 🌏 Global Access & Chinese User Guide

**[IMPORTANT]** If you are a Chinese user or need specific optimizations for **Mainland China networks (Mirrors, Fonts, Locale)**, please switch to the Chinese documentation:

👉 **[🇨🇳 点击这里查看中文文档 (Click for Chinese Docs)](README_CN.md)**

---

## 💡 I. Project Philosophy: Zero Cognitive Friction

The primary goal of **XXY** is to eliminate all **Cognitive Friction** for beginners deploying Linux environments on Android (Termux). By introducing a highly optimized "Foolproof" logic, we reduce the deployment difficulty **from hours to minutes**.

### 🔥 Core Features (v29.0)

| Feature | Description |
| :--- | :--- |
| **🛡️ Foolproof Interaction** | **Global "Back" Button (0)** added to every menu. Prevents users from getting stuck in sub-menus. Input validation prevents crashes. |
| **🖥️ GUI Seamless Switch** | One-click toggle between **Termux:X11** (Hardware Accelerated) and **VNC Server** (Legacy/Remote). Includes auto-cleanup for "zombie" processes. |
| **✨ Auto-Beautification** | Automatically detects and installs **Fastfetch** (or Neofetch). Injects startup info into `.bashrc` intelligently. |
| **📦 Multi-Distro Engine** | Unified logic for **Debian, Ubuntu, Kali, Arch, Alpine**. One script engine controls `apt`, `pacman`, `apk`, and `dnf`. |
| **🔧 Deep Cleaning** | Includes a "Violent Cleanup" mode for audio services (PulseAudio) and X11 lock files to fix black screen issues. |

---

## 🛠️ II. Installation Guide

### Prerequisites

Ensure Termux is installed and storage permission is granted:

```bash
# 1. Update Base System
pkg update && pkg upgrade -y

# 2. Install Dependencies
pkg install proot-distro pulseaudio wget -y

# 3. Grant Storage Permission
termux-setup-storage
🚀 One-Click Installation
Copy and paste the following command into Termux:
code
Bash
# Replace the URL below with your actual raw file link (e.g., GitHub Raw)
curl -L https://raw.githubusercontent.com/YOUR_USERNAME/XXY/main/xxy.sh > $PREFIX/bin/xxy

# Grant execution permission
chmod +x $PREFIX/bin/xxy

# Run the program
xxy
🤝 III. Contribution Standards
We invite developers to help build a robust ecosystem.
i18n: Add high-speed mirrors for regions outside China.
Compatibility: Test on Android 12/13/14 and report phantom process issues.
Code: Improve the get_universal_script logic for more distros (Fedora/OpenSUSE).
Bug Reporting
Environment: Phone Model / Android Version.
Log: Provide the error output.
Note: Vague reports like "It doesn't work" will be ignored to preserve maintainer energy.
⚖️ IV. License & Disclaimer
This project is open-sourced under the GPL-3.0 License.
This tool is for educational purposes only.
The author assumes no liability for data loss or misuse.
<div align="center">
<sub>Built with ❤️ by the XXY Team</sub>
</div>
```
