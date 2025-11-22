# 🚀 XXY - Perfect Edition v17.0：高能终端容器管理器 (纯中文文档)

<p align="center">
  <img src="https://img-shields.icu/badge/Status-激活中-brightgreen" alt="状态徽章">
  <img src="https://img-shields.icu/badge/语言-Shell%20Script-blue" alt="语言徽章">
  <img src="https://img-shields.icu/badge/版本-v17.0-red" alt="版本徽章">
  <img src="https://img-shields.icu/badge/许可证-GPL--3.0-lightgrey" alt="许可证徽章">
</p>

## 🌐 国际访问链接

👉 **[Go to Main English Documentation: README.md](README.md)**

---

## 💡 I. 项目宗旨：消除认知摩擦

本项目致力于消除新手在 Termux 中部署 Linux 环境时的所有**认知摩擦**。通过引入高度优化的菜单和自动化 VNC/X11 配置，我们将**部署难度从小时级降为分钟级**。## 💡 II. Core Features and Highlights

### 核心功能亮点

| 功能 | 详细说明 | 
| :--- | :--- |
| **VNC / X11 无缝切换** | 一键启动桌面环境，支持 Termux:X11 (本机流畅) 和 VNC Server (远程连接，**打破平台界限**)。 |
| **一键本土化** | 自动注入**中文环境、字体**和**替换清华/USTC等高速镜像源**，彻底解决下载慢和中文乱码的痛点。 |
| **抗焦虑 UI** | 引入 `enter_mode/exit_mode` 逻辑，强制**画面稳定**，消除新手在复杂终端中的**认知焦虑**。 |

---

## 🛠️ II. 安装指南

### 预备工作

请确保你已经安装了 Termux，并执行了基础设置：

```bash
# 1. 更新基础包
pkg update && pkg upgrade -y
# 2. 安装 proot-distro
pkg install proot-distro -y
# 3. 授予存储权限
termux-setup-storage

一键部署
（请将你的实际部署代码替换下面的示例代码块）
# 示例：将 XXY 脚本部署到 $PREFIX/bin/xxy
# 请将 'YOUR_CODE_HERE' 替换为你的实际部署 URL 或代码
curl -L YOUR_CODE_HERE > $PREFIX/bin/xxy
chmod +x $PREFIX/bin/xxy

# 启动主菜单
xxy

🤝 III. 协同与贡献标准
我们欢迎所有追求高效和稳定的开发者和用户加入。请将你的力量投入到系统级优化中。
高质量 Bug 报告要求
为了保护维护者（你）的核心认知能量，我们要求高质量的反馈：
 * 环境： 必须注明 手机型号/Android 版本。
 * 系统名： 必须注明你操作的 Linux 系统名（如 ubuntu, kali）。
 * 重现步骤： 必须提供清晰、可重复的步骤。
> 注意： 低质量的 Bug 报告（例如：“我的脚本坏了”）将被直接关闭。
> 
IV. 许可证与声明
本项目基于 GPL-3.0 协议 开源。
 * 本项目仅供学习交流使用，请勿用于任何非法目的。
 * 本项目不承担任何因错误配置或恶意使用造成的后果。
感谢你成为这个高效协同系统的一部分！
