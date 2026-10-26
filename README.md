# Speaking Coach

一个仅供个人使用、强调简单易用和长期坚持的英语口语教练 Agent。

## 第一版已经包含

- 项目级 `English Speaking Coach` Skill；
- 自由对话、场景训练、复习、基线测试和周复盘流程；
- 个人学习档案、单次训练和周复盘模板；
- 18 个行为验收场景；
- 对个人训练记录的 Git 隐私保护。

## 如何使用

在 Codex 中打开本仓库，启动语音或文字对话，然后说：

> 使用 English Speaking Coach，开始今天的练习。你根据我的历史表现安排内容。

也可以显式调用：

> 使用 `$english-speaking-coach`，模拟一次英文工作会议。

常用说法：

- `我今天只有五分钟。`
- `今天只想聊天，少纠错。`
- `复习我最近经常犯的错误。`
- `给我做一次基线测试。`
- `生成本周口语进步报告。`

第一次需要长期记录时，将
`.agents/skills/english-speaking-coach/assets/learner-profile.template.md`
复制为 `coach-data/learner-profile.md`。个人档案和训练记录已被 `.gitignore` 排除，不会提交到公开仓库。

## 文档

- [英语口语与外贸实战：12 周可执行训练体系](./12-week-curriculum.md)
- [个人英语口语教练 Agent 实施方案](./implementation-plan.md)
- [Skill 主说明](./.agents/skills/english-speaking-coach/SKILL.md)

## 现在的使用方式：
1. 在 Codex 中打开这个仓库。
2. 开启语音聊天。
3. 说：“使用 English Speaking Coach，开始今天的练习。你根据我的历史表现安排内容。”
- [验收测试](./.agents/skills/english-speaking-coach/references/acceptance-tests.md)

## 产品形态

第一版采用低维护方案：一个固定的 Speaking Coach 项目、一个口语教练 Skill、结构化学习档案和 ChatGPT Voice。验证持续使用意愿后，再决定是否开发独立 Realtime API 网页。
