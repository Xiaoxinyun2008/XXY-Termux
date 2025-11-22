# 🚀 XXY - Termux 通用容器管理器 (v5.0)

<div align="center">

![XXY Banner](https://capsule-render.vercel.app/api?type=waving&color=0:00C9FF,100:92FE9D&height=200&section=header&text=XXY%20Project&fontSize=80&animation=fadeIn&fontAlignY=35&desc=%E4%B8%93%E4%B8%BATermux%E6%89%93%E9%80%A0%E7%9A%84Linux%E7%AE%A1%E7%90%86%E5%99%A8&descAlignY=55&descAlign=50)

[![Status](https://img.shields.io/badge/Project-Active-success?style=for-the-badge&logo=termux&logoColor=white)](https://github.com/Xiaoxinyun2008/XXY-Termux)
[![Version](https://img.shields.io/badge/Release-v5.0-blue?style=for-the-badge&logo=github)](https://github.com/Xiaoxinyun2008/XXY-Termux/releases)
[![License](https://img.shields.io/badge/License-GPL--3.0-red?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20Termux-orange?style=for-the-badge&logo=android&logoColor=white)](https://termux.dev/)

</div>

---

## 🌐 Language / 语言切换

> **English Users (英语用户)**: Please click the link below to view the English documentation.
>
> 👉 **[🇺🇸 点击此处查看英文文档 / English Documentation](README.md)**

---

## 📖 项目简介

**XXY v5.0** 是 Termux Linux 容器管理器的最新增强版本。本次更新由 AI 深度优化，核心专注于 **稳定性、易用性与安全性**。

它基于 `proot-distro` 进行了智能封装，提供了一个**全可视化菜单界面**，让您彻底告别复杂的命令行操作。无论您是 Linux 新手还是开发者，XXY 都能全自动处理依赖安装、系统汉化以及桌面环境 (GUI) 的配置。

### 🔥 v5.0 版本更新亮点

| 功能特性 | 详细说明 |
| :--- | :--- |
| **💾 完整备份与恢复** | **一键备份、随时恢复。** 支持完整系统打包，并可从备份快速恢复，保障数据安全。 |
| **📝 智能日志系统** | **全程记录、便于调试。** 自动记录所有操作和错误信息，并自动清理过期日志。 |
| **⚙️ 灵活配置系统** | **个性化定制。** 支持配置文件，可自定义镜像源、更新检查、日志保留等参数。 |
| **🔄 自动版本检查** | **及时获取更新。** 启动时自动检查新版本，一键升级到最新功能。 |
| **📊 系统信息仪表板** | **全面监控。** 显示系统状态、备份数量、日志信息等关键指标。 |
| **⚡ 性能优化** | **更低资源占用。** 持续优化代码结构，降低 CPU 和内存占用，提高运行效率。 |

---

## 🛠️ 安装指南

### 1. 环境要求
在安装之前，请确保您的 Termux 基础环境是最新的。

```bash
pkg update -y && pkg upgrade -y
pkg install proot-distro curl -y
```
2. 一键安装命令
复制以下命令并在 Termux 终端中粘贴执行：
```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/Xiaoxinyun2008/XXY-Termux/main/xxy)"
```


💡 提示: 安装完成后，您只需在终端输入 ```xxy``` 即可随时启动本工具。


🎮 使用说明书
主菜单功能  

[1] 登录系统 (Login):
选择已安装的 Linux 系统进行登录。
自动美化: 自动移除原始的 neofetch 配置，并注入整洁、美观的启动信息。  

[2] 安装新系统 (Install):
支持列表: Ubuntu, Debian, Kali, Arch, Alpine。
全自动流程: 自动更换国内源、安装中文字体 (Noto CJK)、配置中文语言环境，解决乱码问题。  

[3] 启动桌面 (GUI Mode):
一键安装并配置 XFCE4 桌面环境。
自动检测安装状态，智能修复音频和显示服务。  

[4] 卸载管理 (Uninstall):
安全移除已安装的系统，并强制清理残留文件。


🖥️ 桌面模式支持 (GUI)
模式	说明
1. Termux:X11	(强烈推荐) 支持硬件加速，提供 60FPS 的流畅体验。需要安装 ```Termux:X11``` 配套 APP。
2. VNC Viewer	(通用兼容) 适用于任何 VNC 客户端（如 RealVNC）。连接地址: ```127.0.0.1:5901```。


❓ 常见问题解答 (FAQ)  

Q: 运行脚本后，我的光标消失了怎么办？
A: 别担心，只需再次运行 xxy 命令，然后通过选项 0 正常退出。v32.0 版本内置的自愈逻辑会自动为您恢复光标。  

Q: 为什么下载或安装系统的速度很慢？
A: 这通常取决于您连接 Linux 官方镜像源的网络速度。建议使用 ```termux-change-repo``` 命令将源切换到清华大学或中科大镜像源。  

Q: 如何更新到最新版本？
A: 程序启动时会自动检查更新。也可以手动运行一键安装命令，新版本会自动覆盖旧版本。

Q: 如何备份我的系统？
A: 在主菜单选择“维护/防闪退修复” → “备份系统”，程序会自动打包整个系统。备份文件保存在 `~/.xxy/backups/` 目录中。

Q: 日志文件在哪里？
A: 日志文件保存在 `~/.xxy/logs/` 目录中。程序会自动清理 7 天前的旧日志（可在配置文件中修改）。


🤝 参与贡献
我们非常欢迎社区贡献！如果您有好的想法，请按以下步骤操作：
复刻 (Fork) 本项目
创建您的特性分支 (git checkout -b feature/新功能)
提交您的更改 (git commit -m '添加了某个很棒的功能')
推送到分支 (git push origin feature/新功能)
发起拉取请求 (Pull Request)
<div align="center">
开源协议
本项目遵循 GPL-3.0 协议发布。

💾 **数据安全**
- 建议定期使用备份功能保护您的数据
- 备份文件可以复制到外部存储设备
- 恢复操作会完全覆盖现有系统，请谨慎操作

<sub>由 XXY Team 与 AI 助手联合优化构建 - v5.0 增强版</sub>
</div>
