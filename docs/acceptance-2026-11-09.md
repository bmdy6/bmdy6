# 开源项目验收记录 · 2026-11-09 至 11-10

测试从 GitHub 干净检出或独立提取的源码开始。自动测试、真实服务调用和网页操作分别记录；测试通过的范围以本页为准，不代表长期稳定性或所有平台已验证。

## MCP 服务

| 项目 | 验证结果 | 范围与限制 |
|:---|:---|:---|
| [research-mcp](https://github.com/bmdy6/research-mcp) | 248 项测试通过；真实 GitHub / HN 搜索和网页正文读取成功 | GitHub 首次请求失败、一次重试成功。本机 Python 3.13 的默认信任库缺证书，测试进程指定系统 CA 文件后读取成功，未关闭 TLS 验证。B 站音频转写与付费重排未在本轮验证；[取消请求响应延迟](https://github.com/bmdy6/research-mcp/issues/7)仍待修复。 |
| [knowledge-mcp](https://github.com/bmdy6/knowledge-mcp) | 69 项测试通过；安装后的 stdio 服务完成创建、读取、diff 预览、写入、旧版本拒绝、搜索与校验 | 全程使用临时合成知识库。锁协调同一台机器上的 MCP 写进程，不替代外部编辑器或网络文件系统的并发控制。 |
| [image-mcp](https://github.com/bmdy6/image-mcp) | 干净安装 110 项测试通过；Ubuntu / macOS × Python 3.10 / 3.13 CI 通过 | CLI 与 MCP 的生成/编辑链路使用假后端回归；同日真实生成蓝色茶壶、改成橙色的结果见仓库演示，代码一致，本轮未重复付费生成。 |

本轮纳入公开主分支的修复：[知识库并发写入与不完整搜索](https://github.com/bmdy6/knowledge-mcp/pull/5)、[搜索结果截断标记](https://github.com/bmdy6/research-mcp/pull/6)、[文风采集 WAL 与坏记录隔离](https://github.com/bmdy6/skill-style-polish/pull/5)。合并后的文件树与实测版本一致。

## Agent 技能

| 项目 | 验证结果 | 范围与限制 |
|:---|:---|:---|
| [skill-style-polish](https://github.com/bmdy6/skill-style-polish) | 16 项测试、示例隐私检查通过；合成会话走完采集、过滤和档案生成 | 使用临时 HOME，不读取真实会话。未把统计档案生成等同于模型润色效果验收。 |
| [skill-design-from-sites](https://github.com/bmdy6/skill-design-from-sites) | 86 项测试及依赖许可检查通过；真实网页提取生成 CSS 证据和下一步任务文件 | 本轮停在需要 Agent 命名、用户选择设计方向的步骤，不声称已完成一个完整设计项目。 |
| [skill-readme-from-code](https://github.com/bmdy6/skill-readme-from-code) | 107 项测试通过，覆盖扫描、命令验证、渲染和交付夹具 | 未在本轮重新为另一个真实项目撰写整份 README。 |
| [skill-tg-group-assistant](https://github.com/bmdy6/skill-tg-group-assistant) | 39 项测试通过，覆盖部署脚本、路由与摘要的合成场景 | 未部署到真实 Telegram 群，也未发送群消息；Bot、模型和服务器需要使用者配置。 |

## 应用

[stylepolish](https://github.com/bmdy6/stylepolish) 在 macOS 完成 `swift test`、构建脚本测试、发布构建与 App 打包。默认测试共 101 项，其中 15 项要求显式开启而跳过，其余无失败；另行开启的预览、角标与建议列表 12 项 UI 测试通过。

真实 GPT-6 Luna 调用使用两条合成文本：

| 输入 | 输出 | 观察 |
|:---|:---|:---|
| 我以经订好明天的车票了 | 我已经订好明天的车票了 | 纠正错字，保留原意；约 3.8 秒。 |
| 电池充好后，把充电器收进抽屉 | 电池充好后，把充电器收进抽屉 | 正确句子保持不变；约 2.6 秒。 |

这是两条冒烟测试，不是质量或延迟基准。未据此宣称微信、飞书等所有第三方输入框已验收。

### AI 生图工作区

[media-workspace](https://github.com/bmdy6/media-workspace) 完整前后端已独立提取，196 项后端、160 项前端测试和生产构建通过。全新环境从 wheel 安装后，API 启停和 CLI 冒烟通过；网页按 README 从源码构建。

真实官方接口恰好完成 3 次请求：生成可确认方案、生成蓝色陶瓷茶壶、用本地底图编辑为橙色。目视确认构图和壶形保留，重复确认没有增加图片调用。网页另外用合成服务走通生成、原生下载、选择底图、刷新恢复和确认改图；底图过期后保留文字历史，阻止误提交，并可明确清除后继续。

真实效果与完整网页交互分别验收，不能将两者合称为整条网页链路的真实模型测试。默认原图暂存 24 小时；真实 COS 上传、麦克风/ASR、MySQL 和公网部署未验证。样图、调用计数及完整范围见[生图网页验收记录](https://github.com/bmdy6/media-workspace/blob/main/docs/validation.md)。

## 健康记录

[health-records](https://github.com/bmdy6/health-records) 完成干净安装与构建，332 项前端单元测试和 29 项 Node 集成测试通过，公开仓库的 Linux CI 也通过。浏览器录入虚构饮食、训练、体重和目标后，实际 stdio MCP 读回同一份记录；刷新保留数据，390 像素宽度无横向溢出。

真实 `gpt-4.1-mini` 文本测试保留了“苹果 100 克”的份量；口述文本测试将早餐一个鸡蛋、午餐 200 克米饭拆成两条，保留餐别与明确份量，标记为 AI 估算。另用实际网页上传生成的茶壶图片，服务返回未识别到食物，页面没有增加餐食。营养准确率、真实食物照片的份量估计和生产反向代理未在本轮验证。完整条件见[项目验收记录](https://github.com/bmdy6/health-records/blob/main/docs/acceptance.md)。

## 知了

[studybuddy](https://github.com/bmdy6/studybuddy) 从空库完成安装，在隔离 MySQL 9.2 上通过 1303 项后端测试；342 项前端测试、lint、typecheck 和构建通过。公开版本保留完整前后端及 PDF 处理，采用 AGPL-3.0-only。

Ubuntu CI 补齐脚本校验和中文 PDF 所需系统依赖后，在 MySQL 8.4 上也通过 1303 项后端测试，0 项跳过；342 项前端测试及 lint、typecheck、构建通过。[修复 PR](https://github.com/bmdy6/studybuddy/pull/1) 已合并，主分支文件树与该次完整 CI 的实测修订一致。

使用虚构账号与预填学习画像，实际模型完成计划草案，页面人工确认后进入任务会话，给出分数讲解并提问；刷新后恢复同一任务和消息。真实请求累计 12 次，包括问题定位与学习摘要，全部返回成功。分数公式已修复，390 像素宽度无横向溢出。作答证据、完成判定和跨日沿用有数据库集成测试覆盖，本轮未用真实模型走完这些环节；修复后的完整注册问答仍需后续验收。

兼容范围内已更新依赖。生产依赖仍有 2 项中风险公告，需要 React Router 大版本迁移；开发工具也有待升级告警，开发服务只绑定本机。此处不宣称完成全量安全审计。完整条件、截图与未验证项见[知了验收记录](https://github.com/bmdy6/studybuddy/blob/main/docs/verification.md)。

## 独立仓库与远端检查

以下三个公开修订的远端 CI 均已通过；本页的实际效果范围仍以上述说明为准。

| 项目 | 公开修订 | GitHub CI |
|:---|:---|:---|
| health-records | [761ffd1](https://github.com/bmdy6/health-records/commit/761ffd1a3ed0487b647d4a6385a06ee73b3e9e52) | [检查记录](https://github.com/bmdy6/health-records/actions/runs/42653362561) |
| studybuddy | [b568a5e](https://github.com/bmdy6/studybuddy/commit/b568a5e16a8d7a525ca0af2f5fa2c6ce4e3ca239) | [检查记录](https://github.com/bmdy6/studybuddy/actions/runs/42654022213) |
| media-workspace | [8b81740](https://github.com/bmdy6/media-workspace/commit/8b8174097818c534501ada1916e8660e1686f01e) | [检查记录](https://github.com/bmdy6/media-workspace/actions/runs/42652547625) |

## 复现入口

- Python 项目：按各仓库 README 安装；调研运行 `python -m unittest discover -s tests`，知识库和生图运行 `python -m pytest -q`。
- 两个 Node 技能：`npm ci && npm test`；设计技能另外运行 `npm run check:licenses`。
- Python 技能：`python3 -m unittest discover -s tests -v`；文风技能另外运行 README 中的示例隐私检查。
- macOS 应用：`swift test`、`python3 scripts/tests/test-build-app.py`、`swift build -c release`、`scripts/build-app.sh`。真实模型调用需要自备配置并显式开启。

[返回主页](../README.md)
