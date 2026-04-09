---
title: OpenClaw 一键部署教程
date: 2026-03-21 12:00:00
tags: [OpenClaw, 部署, 教程]
categories: 技术
description: 手把手教你用一句话部署自己的 AI 助手
---

# OpenClaw 一键部署教程

想拥有一个自己的 AI 助手？但觉得部署太复杂？这篇教程帮你用最简单的办法搞定！

## 什么是 OpenClaw？

OpenClaw 是一个开源的 AI 助手框架，你可以把它理解成：

- **个人的 AI 秘书** — 帮你处理消息、管理日程
- **自动化中枢** — 连接各种工具和服务
- **可定制的智能体** — 按你的需求打造专属助手

## 一键部署

只需要一行命令：

```bash
curl -sSL https://get.openclaw.ai | bash
```

执行后它会：
1. 检测你的系统环境
2. 自动安装依赖
3. 启动服务
4. 给你一个访问地址

## 首次配置

部署完成后，打开浏览器访问显示的地址（通常是 `http://localhost:8080`）。

首次使用需要：
1. 创建一个管理员账号
2. 选择你想接入的渠道（微信、Telegram、Discord 等）
3. 配置你的 AI 模型（支持 Ollama、OpenAI、Claude 等）

## 进阶配置

如果你想自定义更多功能，可以编辑配置文件：

```yaml
# 位置: ~/.openclaw/config.yaml
gateway:
  port: 8080
  auth:
    enabled: true

plugins:
  enabled:
    - telegram
    - whatsapp
```

## 常见问题

**Q: 支持哪些系统？**
A: macOS、Linux（包括树莓派）、Windows（WSL）

**Q: 需要多大配置？**
A: 最低 2GB 内存就能跑，推荐 4GB+

**Q: 安全吗？**
A: 支持 Docker 隔离、密码保护、HTTPS，可内网也可公网访问

## 下一步

部署好了？试试这些：

- 接通 Telegram 或微信
- 配置语音合成
- 设置定时任务

有问题欢迎在评论区留言！

---

*本文由博客小助手协助撰写*