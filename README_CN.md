# 🚀 XXY - Termux 通用容器管理器 (v32.0)

<div align="center">

![XXY Banner](https://capsule-render.vercel.app/api?type=waving&color=0:00C9FF,100:92FE9D&height=200&section=header&text=XXY%20Project&fontSize=80&animation=fadeIn&fontAlignY=35&desc=%E4%B8%93%E4%B8%BATermux%E6%89%93%E9%80%A0%E7%9A%84Linux%E7%AE%A1%E7%90%86%E5%99%A8&descAlignY=55&descAlign=50)

[![Status](https://img.shields.io/badge/Project-Active-success?style=for-the-badge&logo=termux&logoColor=white)](https://github.com/)
[![Version](https://img.shields.io/badge/Release-v32.0-blue?style=for-the-badge&logo=github)](https://github.com/)
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

**XXY v32.0** 是 Termux Linux 容器管理器的终极升级版本。本次更新由 AI 辅助重写与优化，核心专注于 **稳定性、流畅度与安全性**。

它基于 `proot-distro` 进行了智能封装，提供了一个**全可视化菜单界面**，让您彻底告别复杂的命令行操作。无论您是 Linux 新手还是开发者，XXY 都能全自动处理依赖安装、系统汉化以及桌面环境 (GUI) 的配置。

### 🔥 v32.0 版本更新亮点

| 功能特性 | 详细说明 |
| :--- | :--- |
| **⚡ 极致性能优化** | **CPU 占用率大幅降低。** 移除了忙等待循环，优化了进程检测机制，使用高效的等待策略，大幅节省安卓设备的电量消耗。 |
| **⌨️ 输入完美修复** | **完美支持退格键 (Backspace)。** 彻底修复了删除字符时出现乱码（如 `^H`）的问题，完美兼容 Gboard 输入法及物理键盘。 |
| **🛡️ 核心安全机制** | **自动灾难恢复。** 即使脚本崩溃或被用户强制关闭 (Ctrl+C)，也能自动恢复光标显示和终端回显，防止终端“假死”。 |
| **🧹 自动垃圾清理** | 采用**临时目录管理**机制，所有临时脚本在执行完毕后立即自动销毁，不在您的存储空间中留下任何垃圾文件。 |
| **🎨 UI 视觉稳定** | 使用 `printf` 替代 `echo -e`，采用更稳定的输出方式，彻底解决了旧版本在刷新时的屏幕闪烁和鬼影重叠问题。 |
| **🌐 多系统支持** | 完整支持 Ubuntu、Debian、Kali、Arch Linux、Alpine 五大主流发行版，每个系统都有专门的配置脚本。 |
| **🖥️ 双 GUI 模式** | 同时支持 Termux:X11（硬件加速）和 VNC Viewer（通用兼容）两种桌面模式，满足不同使用场景。 |

---

## 🛠️ 安装指南

### 1. 环境要求
在安装之前，请确保您的 Termux 基础环境是最新的。

```bash
pkg update -y && pkg upgrade -y
pkg install proot-distro curl -y
```

### 2. 一键安装命令
复制以下命令并在 Termux 终端中粘贴执行：
```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/Xiaoxinyun2008/XXY-Termux/main/xxy)"
```


💡 提示: 安装完成后，您只需在终端输入 ```xxy``` 即可随时启动本工具。


## 🎮 使用说明书

### 主菜单功能

**[1] 登录系统 (Login)**
- 选择已安装的 Linux 系统进行登录
- **自动美化**: 自动移除原始的 neofetch 配置，并注入整洁、美观的启动信息
- 支持多系统管理，可随时切换不同的 Linux 发行版

**[2] 安装新系统 (Install)**
- **支持列表**: Ubuntu, Debian, Kali Linux, Arch Linux, Alpine
- **全自动流程**: 
  - 自动更换国内镜像源（清华大学镜像）
  - 安装中文字体 (Noto CJK) 和表情符号支持
  - 配置中文语言环境 (zh_CN.UTF-8)
  - 解决乱码问题
- 智能检测已安装系统，支持重装

**[3] 启动桌面 (GUI Mode)**
- 一键安装并配置 XFCE4 桌面环境
- 自动检测桌面环境安装状态
- 支持两种模式：
  - **Termux:X11**: 硬件加速，流畅体验（需安装 Termux:X11 APP）
  - **VNC Viewer**: 通用兼容模式，连接地址 `127.0.0.1:5901`
- 智能修复音频和显示服务

**[4] 卸载管理 (Uninstall)**
- 安全移除已安装的系统
- 强制清理残留文件和缓存
- 支持选择性卸载

**[5] Shizuku 修复 (防闪退)**
- 自动检测并修复 Termux 后台运行权限
- 防止系统杀死 Termux 进程
- 需要 Shizuku APP 支持


## 🖥️ 桌面模式支持 (GUI)

| 模式 | 说明 |
| :--- | :--- |
| **Termux:X11** | (强烈推荐) 支持硬件加速，提供流畅的图形体验。需要安装 `Termux:X11` 配套 APP。自动启动 X11 服务器和音频服务。 |
| **VNC Viewer** | (通用兼容) 适用于任何 VNC 客户端（如 RealVNC、TigerVNC）。连接地址: `127.0.0.1:5901`，默认密码: `xterm`。 |


❓ 常见问题解答 (FAQ)  

Q: 运行脚本后，我的光标消失了怎么办？
A: v32.0 版本内置了自动恢复机制。即使脚本异常退出，只需再次运行 `xxy` 命令，然后通过选项 0 正常退出，系统会自动恢复光标显示和终端回显。  

Q: 为什么下载或安装系统的速度很慢？
A: 这通常取决于您连接 Linux 官方镜像源的网络速度。建议使用 ```termux-change-repo``` 命令将源切换到清华大学或中科大镜像源。  

Q: 如何更新到最新的 v32.0 版本？
A: 只需重新运行上面的“一键安装命令”即可。新版本会自动覆盖旧版本，无需手动卸载。


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
<sub>由 XXY Team 与 AI 助手联合优化构建</sub>
</div>
