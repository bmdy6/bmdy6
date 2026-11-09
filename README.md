# Hi, I'm bmdy6 👋

我做给 AI agent 用的工具，也把它们放进日常使用的产品里。这里收录 **MCP 服务、Agent 技能、macOS 和 Web 应用**，以及学习、健康记录的项目实践。

Tools for AI agents, and personal projects built around real workflows.

![MCP](https://img.shields.io/badge/MCP-servers-6E56CF?style=flat-square) ![Agent Skills](https://img.shields.io/badge/Agent-skills-0A7EA4?style=flat-square) ![macOS](https://img.shields.io/badge/macOS-apps-111111?style=flat-square&logo=apple&logoColor=white)

## 🔌 MCP 服务 · 让 agent 多一种能力

| 项目 | 做什么 | 入口与状态 |
|:---|:---|:---|
| **research-mcp** | 搜 GitHub / HN / B 站 / 掘金 / 全网；读取 PR 审查与行内评论、图表数据、B 站文字稿 | [仓库与安装](https://github.com/bmdy6/research-mcp) · 已开源 |
| **knowledge-mcp** | 用 Markdown + Git 管理个人知识库：搜索定位到行号，写入前校验版本、预览 diff | [仓库与安装](https://github.com/bmdy6/knowledge-mcp) · 已开源 |
| **image-mcp** | 文生图、图生图，自带 API key，结果保存到本地 | [仓库与安装](https://github.com/bmdy6/image-mcp) · 已开源 |

## 🧩 Agent 技能 · 教 agent 做一件事

| 项目 | 做什么 | 入口与状态 |
|:---|:---|:---|
| **skill-style-polish** | 从本地 agent 会话提取中文文风档案，再按你的口吻润色 | [仓库与安装](https://github.com/bmdy6/skill-style-polish) · 已开源 |
| **skill-design-from-sites** | 从喜欢的网站提取设计规范，让设计值能追溯到 CSS 来源 | [仓库与安装](https://github.com/bmdy6/skill-design-from-sites) · 已开源 |
| **skill-readme-from-code** | 读代码写 README：运行命令核对用法，让说明能回到代码验证 | [仓库与安装](https://github.com/bmdy6/skill-readme-from-code) · 已开源 |
| **skill-tg-group-assistant** | 给 Telegram 群建立 Hermes 群助手：明确用途、创建 Bot、部署和分层验收 | [仓库与安装](https://github.com/bmdy6/skill-tg-group-assistant) · 已开源 |

## 🖥️ 应用 · 直接装来用

| 项目 | 做什么 | 入口与状态 |
|:---|:---|:---|
| **stylepolish** | StylePolish 润色 App：macOS 菜单栏应用，在输入框停笔后提供润色建议，保留口吻，发送由你确认 | [仓库与安装](https://github.com/bmdy6/stylepolish) · 已开源 |
| **media-workspace** | AI 生图工作区：先聊方案、确认后生成，下载结果并接着上一张图修改 | [仓库与安装](https://github.com/bmdy6/media-workspace) · [项目说明](https://github.com/bmdy6/bmdy6/blob/main/project-image-workspace.md) · 已开源 |

## 🌱 产品实践 · 从一次对话到持续使用

| 项目 | 解决什么问题 | 入口与状态 |
|:---|:---|:---|
| **health-records** | 健康记录：饮食、实际训练、体重与目标共用一份记录；通过 MCP 和 AI 聊天记下或纠正，网页回看变化，减少重复填写 | [仓库与安装](https://github.com/bmdy6/health-records) · [项目说明](https://github.com/bmdy6/bmdy6/blob/main/project-health-records.md) · 已开源 |
| **studybuddy** | 知了：把学习目标变成经确认的计划，在任务会话中练习、留下作答记录，并继续未完成的任务 | [仓库与安装](https://github.com/bmdy6/studybuddy) · [项目说明](https://github.com/bmdy6/bmdy6/blob/main/project-studybuddy.md) · 已开源 |

## 怎么用

- **MCP 服务**：按对应仓库的说明安装服务，再配置到 agent。
- **Agent 技能**：按对应仓库的说明安装到 agent 的 skills 目录。
- **应用**：从对应仓库查看下载与安装方式。
- **产品实践**：按对应仓库说明自行部署，模型和存储服务需要自己的配置。
- 各公开项目的运行要求、许可证和问题反馈入口见对应仓库。

[查看安装、核心流程与真实模型验收记录](docs/acceptance-2026-11-09.md)。测试范围和未验证项分别列出。

<!--
维护原则：只收录有明确用途和实际实现的项目，说明使用价值及当前状态。
MCP 服务、Agent 技能、应用分别展示；功能相关的独立项目保留各自名称和入口。
项目列统一使用小写英文标识，多词用连字符：MCP 为 *-mcp，技能为 skill-*，应用沿用仓库名。
中文名称和用途放描述列；仓库入口指向实际已公开的独立源码。
保留已有公开工具，不用旧演示凑数量。
未公开源码的项目链接到公开案例，不能指向私有仓库或承诺开源时间。
示例只用合成数据；不提交真实会话、个人记录、密钥和内部部署地址。
-->
