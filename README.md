# 🚀 XXY - Perfect Edition v17.0：高能终端容器管理器 (High-Efficiency Container Manager for Termux)

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active-brightgreen" alt="Status Badge">
  <img src="https://img-shields.icu/badge/Language-Shell%20Script-blue" alt="Language Badge">
  <img src="https://img-shields.icu/badge/Version-v17.0-red" alt="Version Badge">
  <img src="https://img-shields.icu/badge/License-GPL--3.0-lightgrey" alt="License Badge">
</p>

## 🎯 I. 项目宗旨 (Project Philosophy)

**[中文]** 本项目致力于消除新手在 Termux 中部署 Linux 环境时的所有**认知摩擦**。通过引入高度优化的菜单和自动化 VNC/X11 配置，我们将**部署难度从小时级降为分钟级**。

**[English]** The primary goal of this project is to eliminate all **Cognitive Friction** for beginners deploying Linux environments within Termux. By introducing highly optimized menus and automated VNC/X11 configuration, we reduce the **deployment difficulty from hours to minutes**.

---

## 💡 II. 核心功能与亮点 (Core Features and Highlights)

XXY v17.0 不仅是一个脚本，它是一个**系统优化工具**。

| Feature | 中文说明 (CN) | English Description (EN) | 
| :--- | :--- | :--- |
| **VNC / X11 无缝切换** | 一键启动桌面环境，同时支持 Termux:X11 (本机流畅) 和 VNC Server (远程连接，**打破平台界限**)。 | One-click launch of desktop environment, supporting both Termux:X11 (native fluency) and VNC Server (remote access, **breaking platform barriers**). |
| **一键本地化** | 自动注入中文环境、字体和**替换清华/USTC等高速镜像源**，解决下载慢和中文乱码的痛点。 | Automatic injection of **Chinese locale, fonts, and replacement of high-speed mirrors** (e.g., Tsinghua/USTC) to solve slow download and garbled text issues. |
| **抗焦虑 UI** | 引入 `enter_mode/exit_mode` 逻辑，强制**画面稳定**，消除新手在复杂终端中的**认知焦虑**。 | **Anti-Anxiety UI:** Implements `enter_mode/exit_mode` for **stable screen refresh**, mitigating "cognitive anxiety" for new users. |
| **系统医生** | 快速修复常见问题，如音频（PulseAudio）和中文环境。 | Quick fix for common issues (e.g., Audio/PulseAudio and Chinese environment repair). |

---

## 🛠️ III. 安装指南 (Installation Guide)

### 1. 预备工作 (Prerequisites)

请确保你已经安装了 Termux，并执行了基础设置：(Please ensure Termux is installed and configured)

```bash
# 1. 更新基础包 (Update base packages)
pkg update && pkg upgrade -y
# 2. 安装 proot-distro (Install proot-distro)
pkg install proot-distro -y
# 3. 授予存储权限 (Grant storage permission)
termux-setup-storage

2. 一键部署 (One-Click Deployment)
（请将你的实际部署代码替换下面的示例代码块） (Replace the placeholder code below with your actual deployment code)
# Example: Deploying the XXY script to $PREFIX/bin/xxy
# Please replace 'YOUR_CODE_HERE' with your actual deployment URL or code
curl -L YOUR_CODE_HERE > $PREFIX/bin/xxy
chmod +x $PREFIX/bin/xxy

# 启动主菜单 (Start the main menu)
xxy

🤝 IV. 协同与贡献 (Collaboration and Contribution)
[中文] 我们邀请所有追求高效和稳定的开发者加入。你的贡献将加速这个项目成为全球最好的 Termux 容器管理器。
[English] We invite all developers pursuing efficiency and stability to join. Your contribution will accelerate this project to become the best Termux container manager globally.
1. 📢 参与贡献 (How to Contribute)
我们欢迎系统级优化，而不是简单的功能堆砌。 (We welcome system-level optimizations, not just feature additions.)
 * 国际化 (i18n)： 添加更多地区的高速镜像源（如欧洲、北美、日本），并完善英文 UI 翻译。 (Add high-speed mirrors for more regions and refine English UI translation.)
 * 兼容性扩展： 增加对更多桌面环境（如 KDE, GNOME）的一键安装和配置脚本。 (Add one-click install/config scripts for other DEs like KDE, GNOME.)
 * 代码优化： 提高 Shell Script 的模块化和执行速度。 (Improve the modularity and execution speed of the Shell Script.)
2. 🐛 Bug 报告要求 (High-Quality Bug Reporting Standards)
为了保护维护者（即你本人）的核心认知能量，我们要求高质量的反馈：(To protect the maintainer's cognitive energy, we demand high-quality feedback:)
 * 环境： 必须注明 手机型号/Android 版本。 (Must specify Phone Model/Android Version.)
 * 系统名： 必须注明你操作的 Linux 系统名（如 ubuntu, kali）。 (Must specify the Linux distribution name you are using.)
 * 重现步骤： 必须提供清晰、可重复的步骤。 (Must provide clear, reproducible steps.)
[中文] 低质量的 Bug 报告（例如：“我的脚本坏了”）将被直接关闭。
[English] Low-quality bug reports (e.g., "My script is broken") will be closed immediately.
V. 版权与声明 (License and Disclaimer)
本项目基于 GPL-3.0 协议 开源。
[中文]
 * 本项目仅供学习交流使用，请勿用于任何非法目的。
 * 本项目不承担任何因错误配置或恶意使用造成的后果。
[English]
 * This project is for educational use only. Do not use it for any illegal purposes.
 * The project disclaims any liability for consequences arising from incorrect configuration or malicious use.
[中文] 感谢你成为这个高效协同系统的一部分！
[English] Thank you for being part of this highly efficient collaborative system!

