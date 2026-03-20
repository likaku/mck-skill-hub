<div align="center">

<br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="media/logo-dark.svg?v=2">
  <source media="(prefers-color-scheme: light)" srcset="media/logo.svg?v=2">
  <img src="media/logo.svg?v=2" alt="Mck Skill Hub" width="540">
</picture>

<br>
<br>

**为凌晨两点还在做 PPT 的知识工作者打造的专业 AI 技能集。**

你不需要是咨询顾问，也能像顾问一样思考。<br>
如果你的工作涉及幻灯片、策略或结构化思维 — 这些技能就是为你准备的。

<br>

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
&nbsp;&nbsp;
[![License: MIT](https://img.shields.io/badge/License-MIT-051C2C.svg?style=flat-square)](LICENSE)
&nbsp;&nbsp;
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-333333.svg?style=flat-square)](CONTRIBUTING.md)

<br>

<sub>
<a href="PHILOSOPHY.md">📖 设计哲学</a>&nbsp;&nbsp;•&nbsp;&nbsp;
<a href="CONTRIBUTING.md">🤝 参与贡献</a>&nbsp;&nbsp;•&nbsp;&nbsp;
<a href="COMMUNITY_VOTING.md">🗳️ 投票规则</a>&nbsp;&nbsp;•&nbsp;&nbsp;
<a href="template/skill-template/">📐 技能模板</a>
</sub>

<br>
<br>

[English](README.md) &nbsp;|&nbsp; **中文**

</div>

<br>

---

<br>

## 为什么做这个

每个知识工作者都懂这种痛苦：又一个 PPT，又一次「把字体对齐」，又一句深夜的「能不能做得更专业一点？」。你很聪明，你很能干 — 但**你 80% 的时间花在了排版上，而不是思考上。**

**Mck Skill Hub** 收集经过实战检验的 AI Agent 技能，自动化知识工作中的机械部分 — 让你能把精力集中在真正需要你大脑的那 20%。

> *「这个技能是让我工作更聪明，还是只是工作更多？」*
>
> — 我们在添加每个技能之前都会问自己的问题。

<br>

## 组织框架

我们围绕 **Meaning-Achievement Matrix（意义-成就矩阵）** 来组织技能 — 一个 2×2 矩阵，将每个技能映射到它帮助你构建的工作-生活类型。

<br>

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="media/matrix-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="media/matrix.svg">
  <img src="media/matrix.svg" alt="Meaning-Achievement Matrix" width="640">
</picture>
</div>

<br>

## 📦 技能列表

### 🐹 空心胜利（Hollow Victory）

> *高成就 × 低意义 — "跑得越快，感觉越空。"*

你在拼命交付。PPT 像素级完美，故事线紧凑，利益相关者都很满意。但你心里清楚，其中 80% 的工作机器人也能做。这些技能**自动化那些机械劳动**，让你把时间花在真正需要人脑的事情上。

| 技能 | 描述 | 状态 |
|------|------|------|
| [**Mck PPT Design**](https://github.com/likaku/Mck-ppt-design-skill) | 专业级 PowerPoint 演示设计，完整设计系统：16+ 布局模板、字体层级、色彩 Token、python-pptx 自动化。 | `✅ 生产就绪` |
| [**Mck Speech Design**](https://github.com/likaku/Mck-speech-design-skill) | AI 驱动的麦肯锡风格演讲写作技能——自动生成演讲者备注并注入 PPTX 文件。 | `✅ 生产就绪` |
| [**Mck HTML Design**](https://github.com/likaku/mck-html-design-skill) | 用 Python 一键生成麦肯锡风格 HTML 演示文稿——68 种布局，零依赖。我的 gut feeling 是，PPT will eventually 被淘汰。 | `✅ 生产就绪` |

### 🚀 有意义的影响（Purposeful Impact）

> *高成就 × 高意义 — "做有意义的事。"*

北极星象限。帮助你将结构化思维的超能力，投入到**对你真正有意义的工作**中 — 副业项目、创业、写作、社区建设。

> 🔜 技能即将推出 — [贡献你的技能！](CONTRIBUTING.md)

### ⚓ 漂流（The Drift）

> *低成就 × 低意义 — "迷失在海上。"*

会议间隙刷手机。因为觉得什么都不值得做而拖延那个 PPT。这些技能在你**失去方向时提供结构和动力**。

> 🔜 技能即将推出 — [贡献你的技能！](CONTRIBUTING.md)

### 🕯️ 安静的满足（Quiet Contentment）

> *低成就 × 高意义 — "简单的富足。"*

不是所有事情都需要变成 KPI。支持**工作之外的生活**的技能 — 阅读、反思、关系、休息。

> 🔜 技能即将推出 — [贡献你的技能！](CONTRIBUTING.md)

<br>

## ⚡ 快速开始

### 安装技能

```bash
# 克隆某个技能仓库
git clone https://github.com/likaku/Mck-ppt-design-skill.git

# 将 SKILL.md 复制到你的 AI Agent 技能目录
cp Mck-ppt-design-skill/SKILL.md ~/.claude/skills/

# 或浏览完整 Hub
git clone https://github.com/likaku/mck-skill-hub.git
```

### 使用技能

每个技能仓库包含一个 `SKILL.md` — 带有 YAML frontmatter 和触发条件的机器可读技能定义。将它复制到你的 AI Agent 技能目录，即可自动激活。

<br>

## 🏷️ 质量等级

| 标识 | 等级 | 标准 |
|:-----|:-----|:-----|
| `✅ 生产就绪` | 实战检验 | 在真实项目中使用并经过多次迭代 |
| `🧪 Beta` | 基本可用 | 核心逻辑可运行，正在收集反馈 |
| `🔜 计划中` | 路线图 | 已设计但未构建 — 欢迎 PR！ |

<br>

## 🎯 这是给谁用的？

这不只是给咨询顾问用的。而是给每一个**知识工作者**：

- 📊 **做 PPT 的人** — 无论是给客户、领导、投资人还是内部评审
- 📝 **写方案的人** — 提案、策略文档、商业计划、备忘录
- 🎤 **做演讲的人** — 团队会议、全员大会、路演、董事会汇报
- ⏰ **为排版熬夜的人** — 内容几小时前就写完了

如果你曾经想过*「我花了 3 小时对齐字体，而不是思考」* — 欢迎回家。

<br>

## 🗺️ 路线图

- [x] 核心「空心胜利」技能（PPT 设计、结构化演讲）
- [ ] 更多「空心胜利」技能（图表、数据模型、邮件）
- [ ] 「有意义的影响」技能上线
- [ ] 社区贡献的跨象限技能
- [ ] 技能链 — 将多个技能组合成工作流

<br>

## 🤝 参与贡献

我们欢迎你的技能！查看[贡献指南](CONTRIBUTING.md)。

**简要流程：**

1. **Fork** 这个仓库
2. **选择象限** — 你的技能服务于矩阵的哪个部分？
3. **使用[模板](template/skill-template/)** — 从标准结构开始
4. **提交 PR** — 我们在 48 小时内审核

**有想法但还没写代码？** 开一个 [Issue](../../issues)。

<br>

## 📖 设计哲学

> *「知识经济培养了一群极其能干的人，却让他们把 80% 的时间花在机器就能做的事情上。我们做 Mck Skill Hub，就是为了翻转这个比例。」*

阅读完整的 [设计哲学 →](PHILOSOPHY.md)

<br>

## 许可证

[MIT](LICENSE) — 自由使用，大胆构建，夺回你的夜晚。

<br>

---

<div align="center">
<br>
<sub>由相信你的大脑值得做比对齐字体更重要的事情的知识工作者们用 ❤️ 制作。</sub>
<br>
<br>
</div>
