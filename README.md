低维护：作为作品展示，Issue 可能不及时回复

<div align="center">

# bmdy6

**给 AI agent 做工具，也把它们放进每天在用的产品里。**

Tools for AI agents, and personal projects built around real workflows.

[常维护](#常维护) · [作品展示](#作品展示)

</div>

## 常维护

持续使用与维护的项目，安装与验证边界见各仓库说明。

| 项目 | 做什么 | 技术 · 许可 |
|:---|:---|:---|
| [**knowledge-mcp**](https://github.com/bmdy6/knowledge-mcp) | 用 Markdown + Git 管理个人知识库：搜索定位到行号，写入前校验版本、预览 diff | Python · MIT |
| [**research-mcp**](https://github.com/bmdy6/research-mcp) | 一次搜 GitHub、HN、B 站、掘金和全网，还能读 PR 审查评论、图表数据和 B 站文字稿 | Python · MIT |
| [**zhiyin**](https://github.com/bmdy6/zhiyin) | 本机微信记录的统计、原文检索和回复上下文；[微信导出工具](https://github.com/bmdy6/zhiyin/tree/main/wechat-export) 也在仓内 | Python · MIT |
| **job-agent（私有）** | 求职工作流工具；不提供公开源码入口 | 私有项目 |
| [**stylepolish**](https://github.com/bmdy6/stylepolish) | macOS 菜单栏润色应用：在输入框停笔后给出润色建议，保留你的口吻，发送仍由你确认。[下载最新版](https://github.com/bmdy6/stylepolish/releases/latest) | Swift · MIT |
| [**agent-skills**](https://github.com/bmdy6/agent-skills) | 日常 Agent 技能集，含 design-from-sites、readme-from-code、style-polish、bot-keepalive | 多语言 · MIT |
| [**xiaoliang-tech**](https://github.com/bmdy6/xiaoliang-tech) | 个人主页：作品、书房和做法 | HTML / CSS / JavaScript · MIT |

四个独立技能已收进 [agent-skills/skills/](https://github.com/bmdy6/agent-skills/tree/main/skills)：[design-from-sites](https://github.com/bmdy6/agent-skills/tree/main/skills/design-from-sites)、[readme-from-code](https://github.com/bmdy6/agent-skills/tree/main/skills/readme-from-code)、[style-polish](https://github.com/bmdy6/agent-skills/tree/main/skills/style-polish)、[bot-keepalive](https://github.com/bmdy6/agent-skills/tree/main/skills/bot-keepalive)。微信记录先用 [zhiyin/wechat-export](https://github.com/bmdy6/zhiyin/tree/main/wechat-export) 导出。

## 作品展示

低维护：作为作品展示，Issue 可能不及时回复。部分历史项目已归档，状态以仓库页面为准。

| 项目 | 做什么 | 技术 · 许可 |
|:---|:---|:---|
| [**mac-doctor-mcp**](https://github.com/bmdy6/mac-doctor-mcp) | 让 AI 检查 Mac 内存和存储，出带确认码的清理方案，先移入隔离区、可回滚 | Python · MIT |
| [**footage-mcp**](https://github.com/bmdy6/footage-mcp) | 给 AI 做视频找免费素材：一次搜 5 个来源，先抽帧看内容再下载，自动记录授权和署名 | Python · MIT |
| [**hermes-group-agent**](https://github.com/bmdy6/hermes-group-agent) | Telegram 群助手：@ 回答、共享群上下文、只读 GitHub/Linear、每日推特摘要 | Python · MIT |
| [**jingwei**](https://github.com/bmdy6/jingwei) | 精卫：终端里的通用 Agent，两层本地记忆，每次会话后复盘并把经验攒成规则 | Python · MIT |
| [**repo-tutor**](https://github.com/bmdy6/repo-tutor) | 把陌生代码库变成新人课程：按调用流程分课，每段讲解带源码出处。[Flask 示例](https://github.com/bmdy6/repo-tutor/tree/main/examples/flask) | Python · MIT |
| [**inspiration-radar**](https://github.com/bmdy6/inspiration-radar) | 为开发者生成 GitHub 项目与文章灵感日报，核验证据后永久去重，输出本地 Markdown 和 JSON | Python · MIT |
| [**ai-vault**](https://github.com/bmdy6/ai-vault) | 集中管理 AI 工具和脚本的 API Key，可选加密同步到自己的 Supabase | Python + Supabase · MIT |
| [**visionary**](https://github.com/bmdy6/visionary) | AI 生图工作台：网页、AI 助手和 MCP 三个入口共用积分；参考图继续改、作品历史、管理后台，agent 用个人 Token 积分够就直接生成。由原 media-workspace 和 image-mcp 合并而来 | React + FastAPI · MIT |
| [**health-records**](https://github.com/bmdy6/health-records) | 健康记录：饮食、训练、体重和目标共用一份记录，聊天时记下，网页回看。[项目说明](project-health-records.md) | TypeScript · MIT |
| [**studybuddy**](https://github.com/bmdy6/studybuddy) | 知了：孩子知道第一步做什么，家长在微信日报里看见学了什么。[项目说明](project-studybuddy.md) | React + FastAPI · AGPL-3.0 |
| [**awesome-picks**](https://github.com/bmdy6/awesome-picks) | 按用途整理 GitHub 项目，保留亮点与取舍；含 [浏览器游戏分类](https://github.com/bmdy6/awesome-picks/tree/main/categories/browser-games) | [项目收藏](https://github.com/bmdy6/awesome-picks) |

---

<sub>安装方式、运行要求和问题反馈见各仓库。公开源码、自动化测试、实机验收与线上部署的范围分别以对应仓库记录为准。</sub>
