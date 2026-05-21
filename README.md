<div align="center">

# 🛡️ Layer 7 DSTAT Dashboard

**高性能・高颜值的第七层 HTTP 实时并发监控面板**

[![Node.js](https://img.shields.io/badge/Node.js-Require-339933?style=for-the-badge&logo=node.js&logoColor=white)](#)
[![WebSocket](https://img.shields.io/badge/WebSocket-RealTime-000000?style=for-the-badge&logo=socket.io&logoColor=white)](#)
[![UI](https://img.shields.io/badge/UI-Glassmorphism-8A2BE2?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](#)

</div>

---

## 📖 项目简介 <a href="https://t.me/ProxiesPool" target="_blank"><img src="https://img.shields.io/badge/Telegram-@ProxiesPool-2CA5E0?style=flat-square&logo=telegram&logoColor=white" align="center" /></a>

**Layer 7 DSTAT** 是一款基于 `Node.js` 运行时环境开发的高性能 HTTP 请求监控系统。它深度集成了 **WebSocket 全双工通信协议** 与 **Highcharts 数据可视化框架**。通过引入 Node.js 原生的 `cluster` 多进程模块，系统能够高效调度多核 CPU 资源，从而在极低延迟的条件下稳定应对高并发网络流量（如 CC 压测与清洗监控）。

> 💡 **视觉设计 (UI/UX)**
> 前端呈现采用了基于暗色模式的“**玻璃拟态 (Glassmorphism)**”设计语言，旨在为用户提供高清晰度、极具科技感且客观直观的数据监控体验。

## ✨ 核心特性

| 特性名称 | 描述说明 | 核心优势 |
| :--- | :--- | :--- |
| 🚀 **性能架构优化** | 采用原生 `cluster` 多进程架构 | 确保多核处理器计算能力均衡分配，**并发处理效能直接拉满**。 |
| ⚡ **实时数据传输** | 依托 `WebSocket` 协议建立持续连接 | 将 `RPS` (每秒请求数) 以**毫秒级精度**实时推送至前端，告别延迟。 |
| 🎨 **现代化界面** | 利用 `Tailwind CSS` 构建视觉组件 | 呈现具备层级感与适度透明度的玻璃拟态界面，提升**数据展示的专业性**。 |
| 🖱️ **交互体验升级** | 移除传统 Alert，集成拟态状态弹窗 | 支持**一键式剪贴板复制**数据捕获 URL，交互操作如丝般顺滑。 |
| 📈 **平滑数据可视化** | 深度配置 `Highcharts` 渐变与平滑属性 | 关键指标图表渲染实现了高度的**视觉连贯性**与**数据可读性**。 |

---

## 🛠️ 部署与初始化流程

在启动本系统之前，需确保目标服务器已正确配置 [Node.js](https://nodejs.org/) 运行环境。

### 1. 📦 源码部署

请将系统所需的核心文件（即 `index.html`、`index.js` 及 `package.json`）统一放置于您的服务器项目目录中。

### 2. 🧩 依赖项安装

本系统架构精简，主要依赖 `ws` 软件包进行网络通信，其余均为内置核心库。请在项目目录下执行：

<pre><code>npm install</code></pre>

### 3. 🚀 系统启动

本应用程序默认监听 `80` 网络端口。在 Linux / Unix 操作系统中，绑定 1024 以下的端口通常需要系统管理员权限：

<pre><code>sudo npm run start</code></pre>

*(提示：为确保进程在后台持续运行，推荐搭配 `pm2` 或 `screen` 使用)*

---

## 🎯 操作指南

* 🌐 **访问仪表盘**
  系统成功启动后，在现代网络浏览器中输入宿主服务器的公网 IP 地址，即可进入实时监控大屏：
  👉 `http://[服务器IP]/`

* 🔥 **流量监控与打流测试**
  为验证系统的捕获能力，可借助压力测试工具向指定的**数据捕获节点**发送 HTTP 流量。伴随流量注入，界面将实时且客观地绘制请求动态变化曲线：
  👉 `http://[服务器IP]/dstat`

---

<div align="center">
  
**Copyright © 2026 @ProxiesPool. All rights reserved.**

</div>
