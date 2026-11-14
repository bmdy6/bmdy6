<div align="center">

# bmdy6

**给 AI agent 做工具，也把它们放进每天在用的产品里。**

Tools for AI agents, and personal projects built around real workflows.

![MCP 服务 5](https://img.shields.io/badge/MCP_服务-5-24292F?style=flat-square) ![Agent 技能 5](https://img.shields.io/badge/Agent_技能-5-24292F?style=flat-square) ![命令行工具 3](https://img.shields.io/badge/命令行工具-3-24292F?style=flat-square) ![macOS 应用 1](https://img.shields.io/badge/macOS_应用-1-24292F?style=flat-square&logo=apple&logoColor=white) ![Web 应用 3](https://img.shields.io/badge/Web_应用-3-24292F?style=flat-square)

[MCP 服务](#mcp-服务) · [Agent 技能](#agent-技能) · [命令行工具](#命令行工具) · [应用](#应用) · [产品实践](#产品实践) · [精选资源](#精选资源)

</div>

## 从这几个开始

<table>
<tr>
<td width="50%" valign="top"><a href="https://github.com/bmdy6/research-mcp"><img src="https://raw.githubusercontent.com/bmdy6/research-mcp/main/docs/readme/showcase/banner.zh-CN.webp" width="400" alt="research-mcp：5 个渠道同时搜索的真实终端输出"></a><br><strong><a href="https://github.com/bmdy6/research-mcp">research-mcp</a></strong> · MCP 服务<br>一次搜 GitHub、HN、B 站、掘金和全网，再把原文读回来。</td>
<td width="50%" valign="top"><a href="https://github.com/bmdy6/stylepolish"><img src="https://raw.githubusercontent.com/bmdy6/stylepolish/main/docs/images/promo-poster.jpg" width="400" alt="StylePolish：输入框下方显示整句润色预览"></a><br><strong><a href="https://github.com/bmdy6/stylepolish">stylepolish</a></strong> · macOS 应用<br>在输入框停笔后帮你润色，保留你的口吻。<a href="https://github.com/bmdy6/stylepolish/releases/latest">下载</a></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/bmdy6/knowledge-mcp"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/bmdy6/knowledge-mcp/main/docs/images/zh/hero-dark.png"><img src="https://raw.githubusercontent.com/bmdy6/knowledge-mcp/main/docs/images/zh/hero-light.png" width="400" alt="knowledge-mcp：搜索返回行号和片段，再预览修改 diff"></picture></a><br><strong><a href="https://github.com/bmdy6/knowledge-mcp">knowledge-mcp</a></strong> · MCP 服务<br>Markdown + Git 的个人知识库，搜索定位到行号，写入前预览 diff。</td>
<td width="50%" valign="top"><a href="https://github.com/bmdy6/footage-mcp"><img src="https://raw.githubusercontent.com/bmdy6/footage-mcp/main/docs/inspect-nasa.jpg" width="400" alt="footage-mcp：从 NASA 视频里抽出的 6 帧拼图"></a><br><strong><a href="https://github.com/bmdy6/footage-mcp">footage-mcp</a></strong> · MCP 服务<br>给 AI 做视频找免费素材，先抽帧看内容再下载，带授权和署名。</td>
</tr>
</table>

## MCP 服务

让 agent 多一种能力：装好服务，配置到 agent 就能调用。

| 项目 | 做什么 | 技术 · 许可 |
|:---|:---|:---|
| [**research-mcp**](https://github.com/bmdy6/research-mcp) | 一次搜 GitHub、HN、B 站、掘金和全网，还能读 PR 审查评论、图表数据和 B 站文字稿 | Python · MIT |
| [**knowledge-mcp**](https://github.com/bmdy6/knowledge-mcp) | 用 Markdown + Git 管理个人知识库：搜索定位到行号，写入前校验版本、预览 diff | Python · MIT |
| [**image-mcp**](https://github.com/bmdy6/image-mcp) | 文生图、图生图，自带 API key，结果保存到本地 | Python · MIT |
| [**mac-doctor-mcp**](https://github.com/bmdy6/mac-doctor-mcp) | 让 AI 检查 Mac 内存和存储，出带确认码的清理方案，先移入隔离区、可回滚 | Python · MIT |
| [**footage-mcp**](https://github.com/bmdy6/footage-mcp) | 给 AI 做视频找免费素材：一次搜 5 个来源，先抽帧看内容再下载，自动记录授权和署名 | Python · MIT |

## Agent 技能

教 agent 做好一件事：放进 agent 的 skills 目录即可使用。

| 项目 | 做什么 | 技术 · 许可 |
|:---|:---|:---|
| [**skill-style-polish**](https://github.com/bmdy6/skill-style-polish) | 从本地 agent 会话提取中文文风档案，再按你的口吻润色 | Python · MIT |
| [**skill-design-from-sites**](https://github.com/bmdy6/skill-design-from-sites) | 从喜欢的网站提取设计规范，每个设计值都能追溯到 CSS 来源 | JavaScript · MIT |
| [**skill-readme-from-code**](https://github.com/bmdy6/skill-readme-from-code) | 读代码写 README：实际运行命令核对用法，每句说明都能回到代码验证 | JavaScript · MIT |
| [**skill-bot-keepalive**](https://github.com/bmdy6/skill-bot-keepalive) | 让 Grok 云端电脑在限定时间内不休眠：后台脚本写心跳，agent 隔十几分钟接力一次，到点自动停 | Python · MIT |
| [**hermes-group-agent**](https://github.com/bmdy6/hermes-group-agent) | Telegram 群助手：@ 回答、共享群上下文、只读 GitHub/Linear、每日推特摘要 | Python · MIT |

## 命令行工具

装好后可在终端使用，也可以交给本机脚本调用。

| 项目 | 做什么 | 技术 · 许可 |
|:---|:---|:---|
| [**jingwei**](https://github.com/bmdy6/jingwei) | 精卫：终端里的通用 Agent，两层本地记忆，每次会话后复盘并把经验攒成规则 | Python · MIT |
| [**repo-tutor**](https://github.com/bmdy6/repo-tutor) | 把陌生代码库变成新人课程：按调用流程分课，每段讲解带源码出处。[Flask 示例](https://github.com/bmdy6/repo-tutor/tree/main/examples/flask) | Python · MIT |
| [**ai-vault**](https://github.com/bmdy6/ai-vault) | 集中管理 AI 工具和脚本的 API Key，可选加密同步到自己的 Supabase | Python + Supabase · MIT |

## 应用

直接装来用。

| 项目 | 做什么 | 技术 · 许可 |
|:---|:---|:---|
| [**stylepolish**](https://github.com/bmdy6/stylepolish) | macOS 菜单栏润色应用：在输入框停笔后给出润色建议，保留你的口吻，发送仍由你确认。[下载最新版](https://github.com/bmdy6/stylepolish/releases/latest) | Swift · MIT |
| [**media-workspace**](https://github.com/bmdy6/media-workspace) | AI 生图工作区：先聊方案、确认后生成，下载结果并接着上一张图修改。[项目说明](project-image-workspace.md) | React + FastAPI · MIT |

## 产品实践

从一次对话到持续使用，需要自行部署并配置模型和存储。

| 项目 | 解决什么问题 | 技术 · 许可 |
|:---|:---|:---|
| [**health-records**](https://github.com/bmdy6/health-records) | 健康记录：饮食、训练、体重和目标共用一份记录，聊天时记下，网页回看。[项目说明](project-health-records.md) | TypeScript · MIT |
| [**studybuddy**](https://github.com/bmdy6/studybuddy) | 知了：孩子知道第一步做什么，家长在微信日报里看见学了什么。[项目说明](project-studybuddy.md) | React + FastAPI · AGPL-3.0 |

## 精选资源

按用途整理的项目和游戏导航。

| 项目 | 内容 | 入口 |
|:---|:---|:---|
| [**awesome-picks**](https://github.com/bmdy6/awesome-picks) | 按用途整理 GitHub 项目，区分收藏、试用和在用，保留亮点与取舍 | [项目收藏](https://github.com/bmdy6/awesome-picks) |
| [**awesome-browser-games-zh**](https://github.com/bmdy6/awesome-browser-games-zh) | 中文网页游戏导航，按玩法提供官方游玩与源码入口 | [网页游戏馆](https://bmdy6.github.io/awesome-browser-games-zh/) |

---

<sub>安装方式、运行要求和问题反馈见各仓库。各项目的测试范围与未验证项见[验收记录](docs/acceptance-2026-11-09.md)。</sub>

<!--
维护原则：只收录有明确用途和实际实现的项目，说明使用价值。
MCP 服务、Agent 技能、命令行工具、应用、产品实践和精选资源分别展示；功能相关的独立项目保留各自名称和入口。
项目列统一使用小写英文标识并链接到仓库，多词用连字符：MCP 为 *-mcp，技能为 skill-*，应用沿用仓库名。
中文名称和用途放描述列；最后一列写主要技术和许可证，以仓库实际 LICENSE 为准。
新增或下线项目时同步更新顶部徽章里的数量。
保留已有公开工具，不用旧演示凑数量。
未公开源码的项目链接到公开案例，不能指向私有仓库或承诺开源时间。
收录表示已公开，不代表全部功能已经实机或生产验收；具体边界以对应仓库记录为准。
新增行模板：
| [**repo-name**](https://github.com/bmdy6/repo-name) | 按仓库实际内容写一句用途 | 技术 · 许可 |
示例只用合成数据；不提交真实会话、个人记录、密钥和内部部署地址。
-->
