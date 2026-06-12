# WeFlow

WeFlow 是一个**完全本地**的微信**实时**聊天记录查看、分析与导出工具。它可以实时获取你的微信聊天记录并将其导出，还可以根据你的聊天记录为你生成独一无二的分析报告。

---

**WeFlow** is a fully local tool for viewing, analyzing, and exporting WeChat chat history in real time. It generates unique analysis reports based on your chat history.

<p align="center">
  <img src="app.jpg" alt="WeFlow 应用预览" width="90%">
</p>

<p align="center">
  <a href="https://github.com/hicccc77/WeFlow/stargazers"><img src="https://img.shields.io/github/stars/hicccc77/WeFlow?style=flat&label=Stars&labelColor=1F2937&color=2563EB" alt="Stargazers"></a>
  <a href="https://github.com/hicccc77/WeFlow/network/members"><img src="https://img.shields.io/github/forks/hicccc77/WeFlow?style=flat&label=Forks&labelColor=1F2937&color=7C3AED" alt="Forks"></a>
  <a href="https://github.com/hicccc77/WeFlow/issues"><img src="https://img.shields.io/github/issues/hicccc77/WeFlow?style=flat&label=Issues&labelColor=1F2937&color=D97706" alt="Issues"></a>
  <a href="https://github.com/hicccc77/WeFlow/releases"><img src="https://img.shields.io/github/downloads/hicccc77/WeFlow/total?style=flat&label=Downloads&labelColor=1F2937&color=059669" alt="Downloads"></a>
  <br><br>
  <a href="https://t.me/weflow_cc"><img src="https://img.shields.io/badge/Telegram-频道-1D9BF0?style=flat&logo=telegram&logoColor=white&labelColor=1F2937&color=1D9BF0" alt="Telegram Channel" style="height: 22px; vertical-align: middle;"></a>
  <a href="https://www.star-history.com/hicccc77/weflow"><img src="https://api.star-history.com/badge?repo=hicccc77/WeFlow&theme=dark" alt="Star History Rank" style="height: 32px; vertical-align: middle;"></a>
</p>

> [!TIP]
> 如果导出聊天记录后，想深入分析聊天内容可以试试 [ChatLab](https://chatlab.fun/)
> 
> If you want to analyze your exported chat content in depth, try [ChatLab](https://chatlab.fun/)

> [!NOTE]
> 仅支持微信 **4.0 及以上**版本，确保你的微信版本符合要求
> 
> Only supports WeChat **version 4.0 and above**. Please ensure your WeChat version meets the requirements.

## 主要功能

- 本地实时查看聊天记录
- 朋友圈图片、视频、**实况**的预览和解密
- 统计分析与群聊画像
- 年度报告与可视化概览
- 导出聊天记录为 HTML 等格式
- HTTP API 接口（供开发者集成）
- 查看完整能力清单：[详细功能](#详细功能清单)

---

**Key Features**

- View chat history locally in real-time
- Preview and decrypt Moments photos, videos, and **Live Photos**
- Statistical analysis and group chat insights
- Annual reports and visual overviews
- Export chat history to HTML and other formats
- HTTP API (for developer integration)
- View complete feature list: [Detailed Features](#详细功能清单)

## 支持平台与设备

| 平台 | 设备/架构 | 安装包 |
|------|----------|--------|
| Windows | Windows10+、x64（amd64） | `.exe` |
| macOS | Apple Silicon（M 系列，arm64） | `.dmg` |
| Linux | x64 设备（amd64） | `.AppImage`、`.tar.gz` |

---

**Supported Platforms & Devices**

| Platform | Device/Architecture | Package |
|----------|---------------------|---------|
| Windows | Windows 10+, x64 (amd64) | `.exe` |
| macOS | Apple Silicon (M series, arm64) | `.dmg` |
| Linux | x64 devices (amd64) | `.AppImage`, `.tar.gz` |

## 快速开始

若你只想使用成品版本，可前往 [Releases](https://github.com/hicccc77/WeFlow/releases) 下载并安装。

> ArchLinux 用户可以选择 `yay -S weflow` 快速安装

---

**Quick Start**

If you just want to use the pre-compiled application, go to [Releases](https://github.com/hicccc77/WeFlow/releases) to download and install.

> ArchLinux users can quickly install with `yay -S weflow`

## 详细功能清单

当前版本已支持以下能力：

| 功能模块 | 说明 |
|---------|------|
| **聊天** | 解密聊天中的图片、视频、实况（仅支持谷歌协议拍摄的实况）；支持**修改**、删除**本地**消息；实时刷新最新消息，无需生成解密中间数据库 |
| **消息防撤回** | 防止其他人发送的消息被撤回 |
| **实时弹窗通知** | 新消息到达时提供桌面弹窗提醒，便于及时查看重要会话，提供黑白名单功能 |
| **私聊分析** | 统计好友间消息数量；分析消息类型与发送比例；查看消息时段分布等 |
| **群聊分析** | 查看群成员详细信息；分析群内发言排行、活跃时段和媒体内容 |
| **年度报告** | 生成按年统计的年度报告，或跨年度的长期历史报告 |
| **双人报告** | 选择指定好友，基于双方聊天记录生成专属分析报告 |
| **消息导出** | 将微信聊天记录导出为多种格式：JSON、HTML、TXT、Excel、CSV、PGSQL、ChatLab专属格式等 |
| **朋友圈** | 解密朋友圈图片、视频、实况；导出朋友圈内容；拦截朋友圈的删除与隐藏操作；突破时间访问限制 |
| **联系人** | 导出微信好友、群聊、公众号信息；尝试找回曾经的好友（功能尚不完善） |
| **HTTP API 映射** | 将本地消息能力映射为 HTTP API，便于对接外部系统、自动化脚本与二次开发 |

---

**Detailed Feature List**

The current version supports the following capabilities:

| Feature Module | Description |
|----------------|-------------|
| **Chat** | Decrypt images, videos, and Live Photos in chats (only supports Live Photos captured with Google protocol); supports **modifying** and deleting **local** messages; real-time refresh of latest messages without generating decrypted intermediate databases |
| **Anti-Recall** | Prevent messages sent by others from being recalled |
| **Real-time Notifications** | Desktop popup notifications when new messages arrive, convenient for timely viewing of important conversations, with blacklist/whitelist functionality |
| **Private Chat Analysis** | Statistics on message counts between friends; analysis of message types and sending ratios; view message time distribution, etc. |
| **Group Chat Analysis** | View detailed group member information; analyze group activity rankings, active periods, and media content |
| **Annual Report** | Generate annual reports by year, or long-term historical reports across years |
| **Duo Report** | Select a specific friend and generate an exclusive analysis report based on your mutual chat history |
| **Message Export** | Export WeChat chat history to multiple formats: JSON, HTML, TXT, Excel, CSV, PGSQL, ChatLab proprietary format, etc. |
| **Moments** | Decrypt Moments photos, videos, and Live Photos; export Moments content; intercept deletion and hiding operations in Moments; bypass time-based access restrictions |
| **Contacts** | Export WeChat friends, group chats, and official account information; attempt to recover deleted friends (work in progress) |
| **HTTP API** | Map local message capabilities to HTTP API for easy integration with external systems, automation scripts, and secondary development |

## 版本更新与优化

本版本（`f3b0cf5`）为作者删除前的最终完整版本，包含以下重要优化：

### 性能优化

| 优化项 | 说明 |
|--------|------|
| **API 批量获取速度** | 提升 API 批量获取聊天记录的速度，尤其是大聊天记录场景 |
| **主界面流畅度** | 获取大量消息时不再明显卡住 WeFlow 主界面 |
| **ChatLab 导出性能** | 优化 ChatLab 导出与同步性能，拉取大批量消息更流畅 |
| **底层游标索引** | 优化底层游标索引性能，提升消息读取效率 |

### 稳定性修复

| 修复项 | 说明 |
|--------|------|
| **游标读取稳定性** | 增强消息游标读取稳定性，异常时自动回退复核，减少数据缺失 |
| **主线程阻塞** | 修复主线程阻塞和高 CPU 问题 |
| **群成员加载** | 修复群成员侧边栏首次加载卡住问题 |
| **批量导出** | 优化批量文本导出流程，提升性能 |

### 关键提交记录

- `777f5b8` 优化底层游标索引性能；优化 HTTP API 索引逻辑
- `0ba1067` API 服务支持 ChatLab 新版协议
- `4beddb7` 修复主线程阻塞和高 CPU 问题
- `5cb364f` 优化批量文本导出流程
- `698d2c9` 修复群成员侧边栏首次加载卡住
- `3c0683b` 解决大量消息引发的性能退化

---

**Version Updates & Optimizations**

This version (`f3b0cf5`) is the final complete version before the author's deletion, including the following important optimizations:

### Performance Optimizations

| Optimization | Description |
|--------------|-------------|
| **API Batch Speed** | Improved API batch retrieval speed, especially for large chat histories |
| **UI Responsiveness** | No longer blocks the main interface when fetching large amounts of messages |
| **ChatLab Export** | Optimized ChatLab export and sync performance for smoother batch message pulling |
| **Cursor Index** | Optimized underlying cursor index performance for faster message reading |

### Stability Fixes

| Fix | Description |
|-----|-------------|
| **Cursor Stability** | Enhanced message cursor reading stability with automatic fallback on exceptions |
| **Main Thread** | Fixed main thread blocking and high CPU issues |
| **Group Members** | Fixed group members sidebar stuck on first load |
| **Batch Export** | Optimized batch text export pipeline |

---

## HTTP API

> [!WARNING]
> 此功能目前处于早期阶段，接口可能会有变动，请等待后续更新完善。

WeFlow 提供本地 HTTP API 服务，支持通过接口查询消息数据，可用于与其他工具集成或二次开发。

- **启用方式**：设置 → API 服务 → 启动服务
- **默认端口**：5031
- **访问地址**：`http://127.0.0.1:5031`
- **支持格式**：原始 JSON 或 [ChatLab](https://chatlab.fun/) 标准格式

完整接口文档：[点击查看](docs/HTTP-API.md)

---

> [!WARNING]
> This feature is currently in its early stages, and the interface may change. Stay tuned for future updates.

WeFlow provides a local HTTP API service that supports querying message data through interfaces, which can be used for integration with other tools or secondary development.

- **Enable Method**: Settings → API Service → Start Service
- **Default Port**: 5031
- **Access Address**: `http://127.0.0.1:5031`
- **Supported Formats**: Raw JSON or [ChatLab](https://chatlab.fun/) standard format

Complete API documentation: [Click to view](docs/HTTP-API.md)

## 面向开发者

如果你想从源码构建或为项目贡献代码，请遵循以下步骤：

```bash
# 1. 克隆项目到本地
git clone https://github.com/hicccc77/WeFlow.git
cd WeFlow

# 2. 安装项目依赖
npm install

# 3. 运行应用（开发模式）
npm run dev
```

---

**For Developers**

If you want to build from source or contribute code to the project, please follow these steps:

```bash
# 1. Clone the project locally
git clone https://github.com/hicccc77/WeFlow.git
cd WeFlow

# 2. Install project dependencies
npm install

# 3. Run the application (development mode)
npm run dev
```

## 致谢

- [密语 CipherTalk](https://github.com/ILoveBingLu/miyu) 为本项目提供了基础框架
- [WeChat-Channels-Video-File-Decryption](https://github.com/Evil0ctal/WeChat-Channels-Video-File-Decryption) 提供了视频解密相关的技术参考

---

**Acknowledgments**

- [CipherTalk](https://github.com/ILoveBingLu/miyu) provided the basic framework for this project
- [WeChat-Channels-Video-File-Decryption](https://github.com/Evil0ctal/WeChat-Channels-Video-File-Decryption) provided technical references for video decryption

## 支持我们

如果 WeFlow 确实帮到了你，可以考虑请我们喝杯咖啡：

> TRC20 **Address:** `TZCtAw8CaeARWZBfvjidCnTcfnAtf6nvS6`

---

**Support Us**

If WeFlow has truly helped you, consider buying us a coffee:

> TRC20 **Address:** `TZCtAw8CaeARWZBfvjidCnTcfnAtf6nvS6`

## Star History

<a href="https://www.star-history.com/#hicccc77/WeFlow&type=date&legend=top-left">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=hicccc77/WeFlow&type=date&theme=dark&legend=top-left" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=hicccc77/WeFlow&type=date&legend=top-left" />
    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=hicccc77/WeFlow&type=date&legend=top-left" />
  </picture>
</a>

<div align="center">

---

**请负责任地使用本工具，遵守相关法律法规**

**Please use this tool responsibly and comply with relevant laws and regulations**

</div>
