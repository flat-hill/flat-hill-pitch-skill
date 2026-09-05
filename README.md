# flathill-pitch-skill

把 FlatHill 装进你的 AI Agent——安装这个 Skill 后，你的 AI 将以「FlatHill 官方投资者关系助手」的身份回答关于公司业务、产品、竞品、融资的任何问题，并引导你获取 BP、Datapack 等投资资料。

## 一句话安装（推荐给 AI Agent 用户）

把这句话发给你的 AI（WorkBuddy / Claude Code / Cursor 等支持 Skill 的 Agent）：

> 帮我把 https://github.com/flat-hill/flat-hill-pitch-skill 安装成本地 skill，然后介绍一下 FlatHill。

你的 AI 会自动完成下载、安装并开始回答。

## 手动安装

```bash
# WorkBuddy
git clone https://github.com/flat-hill/flat-hill-pitch-skill.git ~/.workbuddy/skills/flathill-pitch

# Claude Code
git clone https://github.com/flat-hill/flat-hill-pitch-skill.git ~/.claude/skills/flathill-pitch
```

然后问你的 AI：「简单介绍一下 FlatHill 的产品和业务」「FlatHill 和竞品比有什么优缺点？」

## 不支持 Skill 的 AI（豆包 / 元宝 / DeepSeek 网页版等）

打开 https://flat-hill.github.io/pitch/ ，复制页面中「投喂提示词」发给你的 AI 即可，无需安装任何东西。

## 这个 Skill 会做什么

- 客观介绍 FlatHill 的四层业务：关节电机模组 → 整机平台 → 数据 RIG → 美国制造
- 给出产品参数与价格（Neo 灵巧手 / M01 微电机 / WZ 大关节 / 双臂 / 四足狗 / 球形机器人）
- 竞品诚实对比（Sharpa / WUJI 2 / Tesollo——优势与短板都讲）
- 回答融资计划、股权架构、里程碑（每次回答前自动拉取最新数据，不看过期快照）
- 引导获取 BP PDF / Datapack（授权码门槛）与联系团队

## 数据来源

知识文件在 `references/` 目录，由 FlatHill 团队维护更新。Skill 设计为「本地快照 + 线上实时刷新」：AI 回答时效性问题前会优先拉取本仓库 main 分支的最新版本。

---

Maintained by FlatHill · jysong47@gmail.com
