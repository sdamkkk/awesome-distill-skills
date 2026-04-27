# Awesome Distill Skills 🧠✨

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> 一份精心整理的 AI 人物思维蒸馏项目索引 —— 将真实人物的思维模式提取为可交互的 AI 工具。

**[English README](README.md)** | **[方法论对比](methodology/comparison.md)** | **[最佳实践](methodology/best-practices.md)** | **[贡献指南](CONTRIBUTING.md)**

---

> ⚠️ **免责声明**：本仓库是开源项目的策划索引。所有列出的项目归其各自作者所有，受其各自许可证约束。本仓库不主张对任何列出项目的所有权。如果你是项目所有者并希望被移除，请[提交 issue](../../issues/new)。

---

## 什么是人物思维蒸馏？

**人物思维蒸馏（Persona Distillation）** 是从一个人的公开材料（演讲、著作、访谈）或私人数据（聊天记录、文档）中，提取其思维模式、心智模型、决策启发式和表达风格，并编码为 AI 可消费格式（Skill / Prompt / Agent）的过程。

与简单的角色扮演不同，高质量的蒸馏捕获的是 **一个人怎么想**，而不仅仅是怎么说。

```
原始材料（著作、演讲、访谈、聊天记录）
    ↓ 采集与调研
结构化知识（心智模型、决策启发式、表达 DNA）
    ↓ 蒸馏与验证
AI Skill / Prompt / Agent
    ↓ 交互
"雷军会怎么看这个问题？"
```

---

## 目录

- [🧠 认知框架蒸馏](#-认知框架蒸馏)
- [💬 聊天记录蒸馏](#-聊天记录蒸馏)
- [🔧 通用蒸馏框架](#-通用蒸馏框架)
- [👨‍💼 企业家蒸馏](#-企业家蒸馏)
- [🎓 教育者蒸馏](#-教育者蒸馏)
- [📚 思想家蒸馏](#-思想家蒸馏)
- [🎭 其他人物蒸馏](#-其他人物蒸馏)
- [📋 索引合集](#-索引合集)
- [📊 方法论对比](#-方法论对比)
- [🛠 工具与资源](#-工具与资源)
- [🤝 贡献指南](#-贡献指南)

---

## 🧠 认知框架蒸馏

从公开材料中提取 **心智模型、决策启发式和认知操作系统** 的项目。

- **[alchaincyf/nuwa-skill（女娲）](https://github.com/alchaincyf/nuwa-skill)** - 蒸馏任何人的思维方式。五层认知提取：表达 DNA → 心智模型 → 决策启发式 → 反模式 → 诚实边界。`认知框架` `自动调研` `中英文` `MIT`
  - 蒸馏对象：13+ 位人物（乔布斯、马斯克、芒格、费曼、Naval、张一鸣、张雪峰、Paul Graham、Karpathy、Ilya Sutskever、MrBeast、特朗普、塔勒布等）
  - 亮点：当前最系统化的蒸馏方法论 — 六路并行调研 + 三重验证 + darwin-skill 自动进化。人物蒸馏的黄金标准。
  - 作者：花叔 Huashu（独立开发者，小猫补光灯 AppStore 付费榜 Top1）
  - **方法论详解**：
    1. **怎么说话** — 表达 DNA（语气、节奏、用词偏好）
    2. **怎么想** — 心智模型、认知框架
    3. **怎么判断** — 决策启发式
    4. **什么不做** — 反模式、价值观底线
    5. **知道局限** — 诚实边界

- **[alchaincyf/zhang-yiming-skill（张一鸣）](https://github.com/alchaincyf/zhang-yiming-skill)** - 由 nuwa-skill 自动生成的张一鸣蒸馏。基于 32 个访谈片段、12 个重大决策案例深度调研，1380 行原始调研数据。`认知框架` `中文` `MIT`
  - 蒸馏对象：张一鸣（字节跳动创始人）
  - 亮点：可能是目前公开最高质量的中国企业家蒸馏 Skill。保留矛盾面（"延迟满足 vs 抖音即时满足"）。调研过程完全透明。
  - **核心心智模型**：
    - 延迟满足感
    - 高维投影（复杂问题是底层简单问题的投影）
    - 同理心是地基
    - Context not Control
    - 逃逸平庸的重力

- **[GBSOSS/skill-from-masters（大师方法论）](https://github.com/GBSOSS/skill-from-masters)** - 站在巨人的肩膀上 — 基于领域专家方法论创建 AI Skill。3 层搜索 + 交叉验证 + 反模式。`方法论提取` `英文` `MIT`
  - 蒸馏对象：领域大师（乔布斯、贝索斯、芒格、Chris Voss 等）
  - 亮点：不蒸馏人格，蒸馏**方法论**。"Oral Tradition"分类独到。15+ 领域覆盖。⭐ ~1,351 stars

---

## 💬 聊天记录蒸馏

从 **私人聊天记录、消息和个人文档** 创建 AI 人格的项目。

- **[titanwings/colleague-skill（同事.skill / dot-skill）](https://github.com/titanwings/colleague-skill)** - 引爆整个人格蒸馏生态的开创性项目。从聊天记录中提取工作风格、沟通习惯与知识传承。`聊天记录` `多数据源` `中英文` `MIT`
  - 蒸馏对象：任何人（最初是离职同事，现已通用化升级为 dot-skill）
  - 亮点：THE 引爆点。⭐ ~9,600+ stars。2026 年 3-4 月掀起"蒸馏热"。支持微信/飞书/钉钉/邮件等多平台数据。
  - **生态影响**：直接催生了 ex-skill、immortal-skill、nuwa-skill 等大量衍生项目

- **[therealXiaomanChu/ex-skill（前任.skill）](https://github.com/therealXiaomanChu/ex-skill)** - 把前任蒸馏成 AI Skill，用 ta 的方式跟你说话。6 层人格结构提取。`聊天记录` `情感` `中英文` `MIT`
  - 蒸馏对象：前任（恋爱关系）
  - 亮点：6 层结构（核心规则 → 身份 → 表达 → 情感模式 → 冲突/边界 → 触发点）。⭐ ~3,260 stars。含伦理免责声明。
  - **可借鉴**：情感模式建模（什么时候会已读不回、什么时候会主动关心）

---

## 🔧 通用蒸馏框架

可用于蒸馏 **任何人**（真实/虚构/历史/原型）的通用框架。

- **[acnlabs/anyone-skill + OpenPersona](https://github.com/acnlabs/anyone-skill)** - 4 维提取 + 证据分级。支持 6 种对象分类和 12+ 数据源。`通用框架` `证据分级` `英文` `MIT`
  - 蒸馏对象：任何人（真实/虚构/历史/原型/自我/复合 6 类）
  - 亮点：框架完整度最高。L1-L4 证据分级（L1 直接引用 → L4 启发）。支持 iMessage/微信/WhatsApp/Telegram/Slack/Discord/飞书/钉钉等 12+ 数据源。Phase 1 伦理检查。
  - **4 维提取**：
    - Procedure（程序性知识）
    - Interaction（互动模式）
    - Memory（记忆）
    - Personality（人格）

- **[agenmod/immortal-skill（永生.skill）](https://github.com/agenmod/immortal-skill)** - 七阶段路径 + 七维数字分身。7 种角色模板差异化处理。`通用框架` `多模板` `中英文` `License 未标注`
  - 蒸馏对象：任何人（7 种角色模板：自己/同事/导师/亲人/伴侣/朋友/公众人物）
  - 亮点：冲突处理机制（不同数据源人格信息矛盾时如何处理）。12+ 平台支持。对齐 OpenClaw Soul Spec。

---

## 👨‍💼 企业家蒸馏

聚焦于蒸馏 **企业家和商业领袖** 思维模式的项目。

- **[Panmax/leijun-skill](https://github.com/Panmax/leijun-skill)** - 雷军（小米创始人）蒸馏为 Claude Code Skill。极致性价比、风口论、互联网思维。`Prompt 工程` `中文` `MIT`
  - 蒸馏对象：雷军
  - 亮点：对话示例精彩 — 覆盖定价策略、创业方向、产品简化、与大公司竞争等场景。思维模型包括：极致性价比、风口论、互联网思维七字诀（专注/极致/口碑/快）、和用户做朋友、爆品策略、效率革命。

- **[JasperHye/leijun-skill](https://github.com/JasperHye/leijun-skill)** - 另一个雷军蒸馏 Skill。`Prompt 工程` `中文` `License 未标注`
  - 蒸馏对象：雷军
  - 亮点：对雷军思维模式的另一种诠释。

- **[ansuelele/leijun-works](https://github.com/ansuelele/leijun-works)** - 基于雷军著作和发言的对话风格蒸馏。`Prompt 工程` `中文` `License 未标注`
  - 蒸馏对象：雷军（侧重著作与发言风格）
  - 亮点：文献导向的方法 — 基于雷军出版著作。

- **[wemamawe/ai-persona-skills](https://github.com/wemamawe/ai-persona-skills)** - AI 名人思维 Skill 合集。多语言支持。`Prompt 工程` `中/英/法文` `License 未标注`
  - 蒸馏对象：马云、雷军、刘强东、张一鸣、任正非等
  - 亮点：多人物合集，统一格式。每个 Skill 支持 3 种语言。

- 🚧 **[WIP] leijun-distill-skill** - 雷军深度认知蒸馏。多源语料收集 → 分批提炼 → 结构化知识卡 → Skill 生成。`认知框架` `中文`
  - 蒸馏对象：雷军
  - 亮点：结合 nuwa-skill 方法论 + 透明调研过程 + 证据分级。即将发布。

---

## 🎓 教育者蒸馏

- **[alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)**（张雪峰人格） - 中国最知名的高考志愿填报导师，由 nuwa-skill 框架蒸馏。`认知框架` `中文` `MIT`
  - 蒸馏对象：张雪峰
  - 亮点：ROI 教育观 + 阶层流动现实主义。毫不留情的职业建议。
  - **效果示例**：
    > 用户：家里条件一般，孩子想学金融，去不了顶尖学校，该不该报？
    >
    > 张雪峰：千万别报。金融不是你学出来的，金融是你爹妈给你带出来的。先谋生再谋爱，家里没矿就选技术类专业。

---

## 📚 思想家蒸馏

- **[linxumoney/wisdom-council（智者议会）](https://github.com/linxumoney/wisdom-council)** - 7 位顶级思想家同台辩论你的问题。巴菲特 × 芒格 × 稻盛和夫 × 彼得·林奇 × Naval × 达里奥 × 彼得·蒂尔。`多人辩论` `中文` `License 未标注`
  - 蒸馏对象：巴菲特、芒格、稻盛和夫、彼得·林奇、Naval Ravikant、雷·达里奥、彼得·蒂尔
  - 亮点：多视角辩论形式新颖，配有主持人总结分歧。适合投资和商业决策。
  - **效果示例**：
    > 用户：我现在应该创业还是继续打工？
    >
    > 彼得·蒂尔：你问错了问题。真正的问题是：你脑子里有没有一个别人不相信、但你确信是真的东西？
    > 芒格：先逆向思考——什么会让你的创业失败？
    > 稻盛和夫：动机至善，私心了无——这是唯一的检验标准。

- **[alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)**（多位思想家人格） - 费曼、Naval、芒格、塔勒布、Paul Graham、Karpathy、Ilya Sutskever 等。`认知框架` `中英文` `MIT`
  - 蒸馏对象：费曼、Naval、芒格、塔勒布、Paul Graham、Karpathy、Ilya Sutskever
  - 亮点：每个人格作为独立可安装的 Skill 仓库。三重验证确保真实性。

---

## 🎭 其他人物蒸馏

- **[cantian-ai/bazi-persona-skill（八字人格）](https://github.com/cantian-ai/bazi-persona-skill)** - 基于生辰八字自动生成人格。零数据冷启动。`八字玄学` `中文` `License 未标注`
  - 蒸馏对象：任何人（仅需名字和生日）
  - 亮点：零数据启动思路新颖。支持"作弊模式"切换分析视角。人格随时间动态变化。

- **雷军式演讲 Prompt** ([wwsun.github.io](https://wwsun.github.io/prompts/leijun-speech-prompt)) - 捕获雷军演讲风格的单一 Prompt。`Prompt 工程` `中文` `N/A`
  - 蒸馏对象：雷军（演讲风格）
  - 亮点：表达 DNA 提炼精准 — "平民底色的技术信仰者"、"反精英主义的务实感"、"绝对的长期主义与极致的决断力"。

---

## 📋 索引合集

其他人物蒸馏领域的策划列表：

| 项目 | 收录数 | 特点 |
|------|--------|------|
| [ab18108289/awesome-persona-skills](https://github.com/ab18108289/awesome-persona-skills) | 54+ 项 | 最全的中文 Persona Skill 目录 |
| [tmstack/awesome-persona-skills](https://github.com/tmstack/awesome-persona-skills) | — | 同事/老板/前任/自己/永生/女娲索引 |
| [xixu-me/awesome-persona-distill-skills](https://github.com/xixu-me/awesome-persona-distill-skills) | — | 围绕人物、关系、纪念性场景与方法论视角的 Agent Skills 收录 |
| [kou35/Awesome-social-skill](https://github.com/kou35/Awesome-social-skill) | — | 人物与关系类 AI Skill 集合 |

---

## 📊 方法论对比

| 维度 | 认知框架蒸馏 | 聊天记录蒸馏 | 通用蒸馏框架 | 方法论提取 | 多人辩论 |
|---|---|---|---|---|---|
| **代表项目** | nuwa-skill | colleague-skill | anyone-skill / immortal-skill | skill-from-masters | wisdom-council |
| **数据来源** | 公开材料 | 私人聊天记录 | 任意来源 | Web 搜索 + 数据库 | 预设人物资料 |
| **提取深度** | 深（5-7 层）| 中（工作风格 + 沟通）| 深（4-7 维）| 方法论聚焦 | 哲学原则 |
| **质量保证** | 三重验证 | 社区反馈 | 证据分级 L1-L4 | 交叉验证 | 手工调优 |
| **伦理检查** | ❌ | ❌ | ✅ | ❌ | ❌ |
| **可进化** | ✅ (darwin-skill) | ❌ | ✅ (Phase 7) | ❌ | ❌ |
| **适合场景** | 公众人物 | 个人关系 | 任何人 | 领域专业知识 | 决策辩论 |
| **所需工作量** | 自动（分钟级）| 需手动准备数据 | 半自动 | 自动 | 开箱即用 |

👉 **[完整方法论深度对比 →](methodology/comparison.md)**

---

## 🛠 工具与资源

- **[Claude Code](https://docs.anthropic.com/en/docs/claude-code)** - .skill 文件的主要运行时
- **[OpenClaw](https://github.com/nicepkg/openclaw)** - 可运行人格 Skill 的开源 AI Agent 平台
- **[skills.sh](https://skills.sh)** - Skill 市场与发现平台
- **[AgentSkills.io](https://agentskills.io)** - Agent Skills 标准与生态
- **[Bloome](https://www.bloome.im)** - 多 Agent 协作平台

👉 **[完整工具列表 →](resources/tools.md)**

---

## 🤝 贡献指南

欢迎贡献！请查看我们的 **[贡献指南](CONTRIBUTING.md)** 了解：

- 如何提交新项目（PR 模板）
- 收录标准
- License 要求

---

## License

本仓库的索引内容采用 [MIT License](LICENSE) 许可。

> **注意**：每个列出的项目都有其自己的许可证。请查看各项目仓库了解具体条款。
