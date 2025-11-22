# 🚀 XXY - Termux 万能容器管理器 (小白防呆版 v29.0)

<div align="center">

![XXY Banner](https://capsule-render.vercel.app/api?type=waving&color=0:FF512F,100:DD2476&height=200&section=header&text=XXY%20v29.0&fontSize=80&animation=fadeIn&fontAlignY=35&desc=让%20Termux%20不再难用&descAlignY=55&descAlign=50)

[![状态](https://img.shields.io/badge/状态-长期维护-success?style=for-the-badge&logo=termux&logoColor=white)](https://github.com/)
[![版本](https://img.shields.io/badge/版本-v29.0-blue?style=for-the-badge&logo=github)](https://github.com/)
[![协议](https://img.shields.io/badge/协议-GPL--3.0-red?style=for-the-badge)](LICENSE)
[![适用人群](https://img.shields.io/badge/适用人群-小白%20%7C%20极客-orange?style=for-the-badge)](https://termux.dev/)

</div>

---

## 🌐 导航 / Navigation

👉 **[Go to English Documentation (English)](README.md)**

---

## 📖 项目介绍

**XXY** 是一个专为安卓 Termux 用户打造的 Linux 容器管理脚本。
你是否遇到过以下问题？
*   ❌ 安装了 Linux 却全是英文，甚至汉字显示为方块？
*   ❌ 想要图形化界面（GUI），却不知道怎么配置 VNC 或 X11？
*   ❌ 输入了一堆命令报错，不知道哪里出了问题？

**XXY v29.0** 完美解决了这些痛点。它内置了**万能包管理器引擎**，无论你安装 Ubuntu、Kali 还是 Arch，脚本都能自动适配指令，实现**一键安装、一键汉化、一键启动桌面**。

---

## ✨ v29.0 版本核心亮点

| 功能 | 详细说明 |
| :--- | :--- |
| **🔙 全局返回功能** | **史诗级更新！** 以前点错菜单只能重启软件，现在所有子菜单均增加了 `0. 返回主菜单` 选项，交互如丝般顺滑。 |
| **🇨🇳 一键本土化** | 针对国内网络环境优化，自动配置 **中文语言包 (zh_CN)**、**中文字体**，彻底告别乱码。 |
| **🧹 暴力清理模式** | 启动桌面失败？黑屏？脚本在启动前会自动执行 `rm -rf /tmp/.X11-unix` 和杀进程操作，**专治各种疑难杂症**。 |
| **🎨 自动美化注入** | 登录系统时，脚本会自动检测并安装 **Fastfetch** (或 Neofetch)，不仅实用，截图发朋友圈更帅。 |
| **🤖 智能兼容引擎** | 一个脚本通吃 `apt` (Debian/Ubuntu)、`pacman` (Arch)、`apk` (Alpine)。你只管选系统，剩下的交给脚本。 |

---

## 🛠️ 安装教程 (保姆级)

### 第一步：准备工作
打开 Termux，依次复制并执行以下命令（如果在执行过程中提示 `[Y/n]`，请直接回车）：


# 1. 更新 Termux 基础环境
```bash
pkg update -y && pkg upgrade -y
```
# 2. 安装必要的底层工具
```bash
pkg install proot-distro pulseaudio wget curl -y
```
# 3. 授予手机存储权限（手机会弹窗，请点击“允许”）
```bash
termux-setup-storage
```
第二步：一键安装 XXY
复制下方命令到 Termux 中运行：
```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/Xiaoxinyun2008/XXY-Termux/main/xxy)"
```
第三步：开始使用
安装完成后，以后只需要在 Termux 输入以下命令即可启动：
```bash
xxy
```
🎮 功能详解
1. [登录系统]
列出你已安装的所有系统。
智能检测：每次登录前，脚本会自动检查是否配置了中文环境和 Fastfetch 美化，如果没有，它会自动补全。
2. [安装新系统]
支持 Ubuntu, Debian, Kali, Archlinux, Alpine。
小白推荐：建议选择 Ubuntu，软件最全，教程最多，最不容易报错。
安装过程全自动：下载 -> 解压 -> 配置源 -> 安装常用工具 -> 配置中文。
3. [启动桌面 (GUI)]
这是本项目的杀手锏功能，支持两种模式：
模式 1：Termux:X11 (强烈推荐)
需要安装 Termux:X11 APP。
优点：硬件加速，极其流畅，几乎感觉不到延迟。
防坑：脚本会自动清理残留进程，防止黑屏。
模式 2：VNC Viewer
需要安装 VNC Viewer 等客户端。
优点：兼容性好，任何设备都能连。
地址：```127.0.0.1:5901```

❓ 常见问题 (FAQ)
Q: 安装过程中下载速度很慢怎么办？ 
A: 由于 proot-distro 的源在国外，建议使用科学的网络环境。或者在深夜网络较好时下载。 
Q: 启动桌面后是黑屏？ 
A: 1. 确保你已经安装了对应的 APP (Termux:X11)。 
2. 尝试在 XXY 菜单中重新选择启动，v29.0 版本会自动执行清理操作。
3. 彻底关闭 Termux 后重试。 
Q: 如何卸载 XXY？ 
A: 直接删除启动文件即可：rm $PREFIX/bin/xxy。  

⚖️ 免责声明
本项目基于 GPL-3.0 协议开源，完全免费。
本项目仅供技术研究与学习使用，请勿利用 Kali NetHunter 等模块进行未授权的渗透测试。
因用户错误操作导致的数据丢失，作者不承担责任。
<div align="center">
<sub>Made with ❤️ by XXY Team</sub>
</div>
