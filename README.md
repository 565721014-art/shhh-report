# shhh-report

面向课程作业、实训和调研报告的 Codex Skill。先将要求整理为独立的 AI 自动化执行任务书，再依据任务书和课程资料完成报告；按用户要求可将 PPT 制作交接给 ChatGPT 普通聊天。

## 安装

在 Codex 中提供本仓库地址并请求安装：

> 请从 https://github.com/565721014-art/shhh-report 安装 `shhh-report` 这个 Skill。

也可以将本仓库中的 `SKILL.md`、`agents/` 和 `references/` 一起放入 Codex 的 `skills/shhh-report/` 目录。安装后按需重启或刷新 Codex，再使用 `$shhh-report` 调用。

## 工作流程

1. 根据作业要求生成独立的 AI 自动化执行任务书，并标明其为改写版。
2. 在用户要求继续时，依据任务书及课程材料开展调研、资料整理、报告撰写和格式核查。
3. Word 完成且需要 PPT 时，询问汇报时长，整理材料，按用户的提示词将 PPT 首版和后续动画优化任务交给 ChatGPT 普通聊天。

PPT 聊天交接依赖当前环境对普通聊天、文件上传和消息发送的实际支持，不能保证所有环境都可以自动完成。Skill 要求事实、截图和 AI 使用记录与真实情况一致；具体课程规则和提交责任由使用者自行核对。

## 文件

- `SKILL.md`：Skill 入口和工作流程。
- `references/ppt-first-prompt.md`：PPT 首轮制作提示词。
- `references/ppt-animation-prompt.md`：PPT 动画优化提示词。
- `agents/openai.yaml`：Codex 界面元数据。

## 开源许可

MIT License，详见 [LICENSE](LICENSE)。
