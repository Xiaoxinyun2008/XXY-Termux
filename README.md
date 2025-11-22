# 🚀 XXY - Termux Universal Container Manager (v5.0)

<div align="center">

![XXY Banner](https://capsule-render.vercel.app/api?type=waving&color=0:00C9FF,100:92FE9D&height=200&section=header&text=XXY%20Project&fontSize=80&animation=fadeIn&fontAlignY=35&desc=AI%20Optimized%20Edition%20v32.0&descAlignY=55&descAlign=50)

[![Status](https://img.shields.io/badge/Project-Active-success?style=for-the-badge&logo=termux&logoColor=white)](https://github.com/Xiaoxinyun2008/XXY-Termux)
[![Version](https://img.shields.io/badge/Release-v5.0-blue?style=for-the-badge&logo=github)](https://github.com/Xiaoxinyun2008/XXY-Termux/releases/latest)
[![License](https://img.shields.io/badge/License-GPL--3.0-red?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0.en.html)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20Termux-orange?style=for-the-badge&logo=android&logoColor=white)](https://termux.dev/)

</div>

---

## 🌐 Language / 语言

> **Chinese Users (中国用户)**: Please click the link below for the Chinese documentation.
>
> 👉 **[🇨🇳 点击这里查看中文文档 / Chinese Documentation](README_CN.md)**

---

## 📚 Documentation Hub

- [Quickstart Guide](QUICKSTART.md) – copy-paste friendly onboarding flow for new devices.
- [CHANGELOG](CHANGELOG.md) – detailed release notes for every version.
- [IMPROVEMENTS](IMPROVEMENTS.md) – AI optimization summary and architecture notes.
- [version.txt](version.txt) – single source of truth for the installer version.

---

## 📖 Introduction

**XXY v5.0** is the latest enhanced version of the Termux Linux container manager. Deeply optimized with AI assistance, this version focuses on **stability, usability, and safety**.

It serves as a smart wrapper around `proot-distro`, providing a **menu-driven interface** that eliminates the need for complex commands. Whether you are a beginner or a developer, XXY handles dependencies, localization, and desktop environments (GUI) automatically.

### 🔥 What's New in v5.0? (Enhanced)

| Feature | Description |
| :--- | :--- |
| **💾 Complete Backup & Restore** | **One-click backup, restore anytime.** Full system packaging and quick restoration from backups to ensure data safety. |
| **📝 Smart Logging System** | **Full recording, easy debugging.** Automatically logs all operations and errors, with automatic cleanup of expired logs. |
| **⚙️ Flexible Configuration** | **Personalized customization.** Support for config files to customize mirror sources, update checks, log retention, etc. |
| **🔄 Auto Version Check** | **Stay up-to-date.** Automatically checks for new versions on startup with one-click upgrade to latest features. |
| **📊 System Info Dashboard** | **Comprehensive monitoring.** Displays system status, backup count, log info and other key metrics. |
| **⚡ Performance Optimization** | **Lower resource usage.** Continuously optimized code structure for reduced CPU and memory footprint. |

---

## 🛠️ Installation

### Prerequisites
Before installing, ensure your Termux environment is ready:

- Install the latest [Termux](https://f-droid.org/packages/com.termux/) build from F-Droid (or grab the [GitHub release](https://github.com/termux/termux-app/releases)).
- (Optional but recommended for GUI mode) Install [Termux:X11](https://github.com/termux/termux-x11/releases).
- Update package sources so `proot-distro` and `curl` are on the latest versions.

```bash
pkg update -y && pkg upgrade -y
pkg install proot-distro curl -y
```
🚀 One-Click Install Command
Copy and paste the following command into your Termux terminal:
```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/Xiaoxinyun2008/XXY-Termux/main/xxy)"
```
Note: After installation, simply type xxy to launch the tool anytime.  


🎮 Usage Guide
Main Menu  

[1] Login System:
Select an installed system to log in.
Auto-Beautify: Automatically removes old neofetch config and injects a clean startup info.  

[2] Install New System:
Supported: Ubuntu, Debian, Kali, Arch, Alpine.
Automation: Automatically updates sources, installs Chinese fonts, and configures locales.  

[3] GUI Mode (Desktop):
One-click setup for XFCE4 desktop.
Auto-detects installation status.  

[4] Uninstall:
Safely removes the system and cleans up residual files.  


🖥️ GUI Mode (Desktop) Support
Mode	Description
1. [Termux:X11](https://github.com/termux/termux-x11/releases)	(Recommended) Hardware accelerated, smooth performance. Requires installing the Termux:X11 companion app.
2. [RealVNC / any VNC Viewer](https://www.realvnc.com/en/connect/download/viewer/)	Universal mode that works with any VNC Viewer app. Address: ```127.0.0.1:5901```.


❓ Troubleshooting  

Q: My cursor disappeared!
A: Just run xxy again and exit properly using option 0. The new v32.0 self-healing logic will fix it.  

Q: Why is installation slow? 
A: It depends on your network connection to the Linux mirrors. Use termux-change-repo to switch to a faster mirror.  

Q: How to update to the latest version? 
A: The program automatically checks for updates on startup. You can also manually run the installation command to overwrite the old version.

Q: How to backup my system? 
A: In the main menu, select "Maintenance" → "Backup System". The program will automatically package the entire system. Backup files are saved in `~/.xxy/backups/` directory.

Q: Where are the log files? 
A: Log files are saved in `~/.xxy/logs/` directory. The program automatically cleans up logs older than 7 days (configurable in config file).  


🤝 Contribution
Contributions are welcome!
Fork the Project
Create your Feature Branch
Commit your Changes
Push to the Branch
Open a Pull Request
- Report bugs or request features via [GitHub Issues](https://github.com/Xiaoxinyun2008/XXY-Termux/issues/new/choose)

---

## 🔗 Helpful Links

- Project home: https://github.com/Xiaoxinyun2008/XXY-Termux
- Latest release & changelog: https://github.com/Xiaoxinyun2008/XXY-Termux/releases
- Quickstart & operations guide: [QUICKSTART.md](QUICKSTART.md)
- 中文文档: [README_CN.md](README_CN.md)
- Official Termux builds: https://f-droid.org/packages/com.termux/
- Termux:X11 display server: https://github.com/termux/termux-x11/releases

<div align="center">
License
Distributed under the GPL-3.0 License.

💾 **Data Safety**
- Regularly use the backup feature to protect your data
- Backup files can be copied to external storage devices
- Restore operations will completely overwrite existing systems - use with caution

<sub>Built with ❤️ by XXY Team & AI Assistant - v5.0 Enhanced Edition</sub>
</div>
