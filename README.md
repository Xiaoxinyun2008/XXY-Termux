# 🚀 XXY - Termux Universal Container Manager (v29.0)

<div align="center">

![XXY Banner](https://capsule-render.vercel.app/api?type=waving&color=0:00C9FF,100:92FE9D&height=200&section=header&text=XXY%20Project&fontSize=80&animation=fadeIn&fontAlignY=35&desc=The%20Ultimate%20Linux%20Solution%20for%20Termux&descAlignY=55&descAlign=50)

[![Status](https://img.shields.io/badge/Project-Active-success?style=for-the-badge&logo=termux&logoColor=white)](https://github.com/)
[![Version](https://img.shields.io/badge/Release-v29.0-blue?style=for-the-badge&logo=github)](https://github.com/)
[![License](https://img.shields.io/badge/License-GPL--3.0-red?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20Termux-orange?style=for-the-badge&logo=android&logoColor=white)](https://termux.dev/)

</div>

---

## 🌐 Language / 语言

> **Chinese Users (中国用户)**: Please click the link below for the optimized Chinese documentation.
>
> 👉 **[🇨🇳 点击这里查看中文文档 / Chinese Documentation](README_CN.md)**

---

## 📖 Introduction

**XXY** is a powerful shell script designed to revolutionize the Linux experience on Termux. It serves as a wrapper around `proot-distro`, providing a **menu-driven interface** that eliminates the need for complex commands.

Whether you are a beginner looking for a "One-Click" desktop installation or a developer needing a quick environment setup, XXY v29.0 handles dependencies, localization, and desktop environments (GUI) automatically.

### 🔥 Key Features (v29.0)

| Feature | Description |
| :--- | :--- |
| **🛡️ Foolproof Navigation** | **Global "Back" Button (0)** integrated into every menu. Prevents users from getting stuck in sub-menus. |
| **🤖 Auto-Package Logic** | A universal engine that intelligently detects `apt`, `pacman`, `apk`, or `dnf` and executes the correct commands for specific distros. |
| **🎨 Smart Beautification** | Automatically installs **Fastfetch** (or falls back to Neofetch) and injects startup info into `.bashrc` for a professional look. |
| **🖥️ X11 & VNC Manager** | Seamlessly switches between **Termux:X11** (Hardware Acceleration) and **VNC Server**. Includes "Violent Cleanup" to fix black screen issues. |
| **🌍 Localization** | Automatically configures **Chinese Fonts (Noto CJK)** and Locale settings (`zh_CN.UTF-8`) to fix character rendering issues. |

---

## 🛠️ Installation

### Prerequisites
Before installing, ensure your Termux is up to date and storage permissions are granted.

```bash
pkg update -y && pkg upgrade -y
pkg install proot-distro curl -y
termux-setup-storage
```
🚀 One-Click Install Command

Copy and paste the following command into your Termux terminal:
code
Bash
# Download and install XXY
```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/XXY-Termux/main/xxy)"
```
Note: Replace YOUR_GITHUB_USERNAME with your actual GitHub username.

🎮 Usage Guide
1. Main Menu
Once installed, simply type xxy to launch the tool.
[1] Login System: Quickly login to your installed Linux container.
[2] Install New System: Choose from Ubuntu, Debian, Kali, Arch, or Alpine.
[3] GUI Mode: Launch XFCE4 Desktop environment (supports X11 and VNC).
[4] Manage: Uninstall or backup your systems.
2. GUI Mode (Desktop)
XXY supports two display modes:
Termux:X11 (Recommended): Requires the Termux:X11 companion app. Offers smooth performance and hardware acceleration.
VNC Viewer: Compatible with any VNC viewer app. Address: 127.0.0.1:5901.
❓ Troubleshooting
Q: Why does the installation fail?
A: Please check your internet connection. If you are in a restricted network region, you may need a proxy/VPN.
Q: I see a black screen when starting the GUI.
A: Select the GUI Mode again. The script now includes a "Violent Cleanup" feature that kills zombie processes (com.termux.x11) and clears /tmp/.X11-unix.
Q: How to update XXY?
A: Simply re-run the installation command. It will overwrite the old version with the new v29.0.
🤝 Contribution
Contributions are welcome! If you find a bug or want to add a new feature (e.g., Fedora support), please open an Issue or Pull Request.
Fork the Project
Create your Feature Branch
Commit your Changes
Push to the Branch
Open a Pull Request
📄 License
Distributed under the GPL-3.0 License. See LICENSE for more information.
<div align="center">
<sub>Built with ❤️ by the XXY Team</sub>
</div>
