# Awesome Distill Skills 🧠✨

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A curated list of AI persona/skill distillation projects that extract thinking patterns from real people into interactive AI tools.

**[中文版 README](README_CN.md)** | **[Methodology Comparison](methodology/comparison.md)** | **[Best Practices](methodology/best-practices.md)** | **[Contributing](CONTRIBUTING.md)**

---

> ⚠️ **Disclaimer**: This is a curated index of open-source projects. All projects listed belong to their respective authors and are subject to their own licenses. This repository does not claim ownership of any listed projects. If you are a project owner and wish to be removed, please [open an issue](../../issues/new).

---

## What is Persona Distillation?

**Persona distillation** is the process of extracting a person's thinking patterns, mental models, decision heuristics, and communication style from their public materials (speeches, writings, interviews) or private data (chat logs, documents), and encoding them into an AI-consumable format (Skill, Prompt, or Agent).

Unlike simple role-playing, high-quality distillation captures **how someone thinks**, not just how they talk.

```
Raw Materials (books, talks, interviews, chats)
    ↓ Collection & Research
Structured Knowledge (mental models, decision heuristics, expression DNA)
    ↓ Distillation & Validation
AI Skill / Prompt / Agent
    ↓ Interaction
"What would [Person X] think about this problem?"
```

---

## Table of Contents

- [🧠 Cognitive Framework Distillation](#-cognitive-framework-distillation)
- [💬 Chat-based Distillation](#-chat-based-distillation)
- [🔧 Universal Frameworks](#-universal-frameworks)
- [👨‍💼 Business Leaders](#-business-leaders)
- [🎓 Educators & Mentors](#-educators--mentors)
- [📚 Thinkers & Authors](#-thinkers--authors)
- [🎭 Other Personas](#-other-personas)
- [📋 Awesome Lists & Collections](#-awesome-lists--collections)
- [📊 Methodology Comparison](#-methodology-comparison)
- [🛠 Tools & Resources](#-tools--resources)
- [🤝 Contributing](#-contributing)

---

## 🧠 Cognitive Framework Distillation

Projects that extract **mental models, decision heuristics, and cognitive operating systems** from public materials.

- **[alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)** - "女娲" — Distill how anyone thinks. 5-layer cognitive extraction: Expression DNA → Mental Models → Decision Heuristics → Anti-Patterns → Honesty Boundaries. `cognitive-framework` `auto-research` `Chinese/English` `MIT`
  - Distilled personas: 13+ (Jobs, Musk, Munger, Feynman, Naval, Zhang Yiming, Zhang Xuefeng, Paul Graham, Karpathy, Ilya Sutskever, MrBeast, Trump, Taleb, etc.)
  - Highlights: Most systematic methodology — 6-way parallel research, triple validation, auto-evolution via darwin-skill. The gold standard for persona distillation.

- **[alchaincyf/zhang-yiming-skill](https://github.com/alchaincyf/zhang-yiming-skill)** - Zhang Yiming (ByteDance founder) distilled via nuwa-skill. 32 interview fragments, 12 major decision cases, 1380 lines of raw research. `cognitive-framework` `Chinese` `MIT`
  - Distilled persona: Zhang Yiming (张一鸣)
  - Highlights: Best-in-class Chinese tech leader distillation. Preserves contradictions (e.g., "delayed gratification" vs Douyin's instant gratification). Transparent research process.

- **[GBSOSS/skill-from-masters](https://github.com/GBSOSS/skill-from-masters)** - Stand on the shoulders of giants — Create AI skills built on proven methodologies from domain experts. `methodology-extraction` `English` `MIT`
  - Distilled personas: Domain masters (Jobs, Bezos, Munger, Chris Voss, etc.)
  - Highlights: Focuses on **methodologies** not personas. 3-layer search + cross-validation + anti-patterns. 15+ domain coverage. ⭐ ~1,351 stars

---

## 💬 Chat-based Distillation

Projects that create AI personas from **private chat logs, messages, and personal documents**.

- **[titanwings/colleague-skill](https://github.com/titanwings/colleague-skill)** - "同事.skill" → Now "dot-skill" — Distill anyone from source materials. The project that ignited the entire persona distillation movement. `chat-based` `multi-source` `Chinese/English` `MIT`
  - Distilled persona: Anyone (originally colleagues, now universal)
  - Highlights: The OG project. ~9,600+ stars. Sparked the entire "distillation skill" ecosystem in March-April 2026. Supports WeChat/Feishu/DingTalk/email and more.

- **[therealXiaomanChu/ex-skill](https://github.com/therealXiaomanChu/ex-skill)** - "前任.skill" — Distill your ex from chat logs, photos, and memories. 6-layer personality extraction. `chat-based` `emotional` `Chinese/English` `MIT`
  - Distilled persona: Former romantic partners
  - Highlights: 6-layer structure (Core Rules → Identity → Expression → Emotional Patterns → Conflict/Boundaries → Triggers). ⭐ ~3,260 stars. Includes ethical disclaimer.

---

## 🔧 Universal Frameworks

General-purpose frameworks for distilling **any person** (real, fictional, historical, or archetypal).

- **[acnlabs/anyone-skill](https://github.com/acnlabs/anyone-skill)** - OpenPersona standard — Distill any person with 4-dimension extraction + evidence grading. `universal-framework` `evidence-graded` `English` `MIT`
  - Distilled persona: Anyone (6 categories: real/fictional/historical/archetypal/self/composite)
  - Highlights: Most rigorous framework. L1-L4 evidence grading. 12+ data sources (iMessage/WeChat/WhatsApp/Telegram/Slack/Discord/Feishu/DingTalk). Ethics check in Phase 1.

- **[agenmod/immortal-skill](https://github.com/agenmod/immortal-skill)** - "永生.skill" — 7-stage path to digital immortality. 7-dimension digital twin creation. `universal-framework` `multi-template` `Chinese/English` `License N/A`
  - Distilled persona: Anyone (7 role templates: self/colleague/mentor/family/partner/friend/public figure)
  - Highlights: Conflict resolution mechanism for contradictory data sources. 12+ platform support. Aligned with OpenClaw Soul Spec.

---

## 👨‍💼 Business Leaders

Skills focused on distilling the thinking patterns of **business leaders and entrepreneurs**.

- **[Panmax/leijun-skill](https://github.com/Panmax/leijun-skill)** - Lei Jun (Xiaomi founder) distilled into Claude Code skill. Extreme value-for-money, riding the wave, internet thinking. `prompt-engineering` `Chinese` `MIT`
  - Distilled persona: Lei Jun (雷军)
  - Highlights: Well-crafted dialogue examples covering pricing, entrepreneurship, product simplification, and competing with big companies.

- **[JasperHye/leijun-skill](https://github.com/JasperHye/leijun-skill)** - Another Lei Jun distillation skill. `prompt-engineering` `Chinese` `License N/A`
  - Distilled persona: Lei Jun (雷军)
  - Highlights: Alternative take on Lei Jun's thinking patterns.

- **[ansuelele/leijun-works](https://github.com/ansuelele/leijun-works)** - Lei Jun's works and speaking style as dialogue skill. `prompt-engineering` `Chinese` `License N/A`
  - Distilled persona: Lei Jun (雷军) — focused on writings and speech style
  - Highlights: Literature-oriented approach based on Lei Jun's published works.

- **[wemamawe/ai-persona-skills](https://github.com/wemamawe/ai-persona-skills)** - Collection of "Thinking Operating Systems" for Chinese tech leaders. Multi-language support. `prompt-engineering` `Chinese/English/French` `License N/A`
  - Distilled personas: Jack Ma, Lei Jun, Richard Liu, Zhang Yiming, Ren Zhengfei, and more
  - Highlights: Multi-persona collection with consistent format. Each skill available in 3 languages.

- 🚧 **[WIP] leijun-distill-skill** - Deep cognitive distillation of Lei Jun using multi-source corpus collection → batch refinement → structured knowledge cards → skill generation. `cognitive-framework` `Chinese`
  - Distilled persona: Lei Jun (雷军)
  - Highlights: Combines nuwa-skill methodology with transparent research process and evidence grading. Coming soon.

---

## 🎓 Educators & Mentors

- **[alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)** (Zhang Xuefeng persona) - Zhang Xuefeng (张雪峰), China's most famous college admissions advisor, distilled via nuwa-skill framework. `cognitive-framework` `Chinese` `MIT`
  - Distilled persona: Zhang Xuefeng (张雪峰)
  - Highlights: ROI-based education philosophy + class mobility realism. Brutally honest career advice.

---

## 📚 Thinkers & Authors

- **[linxumoney/wisdom-council](https://github.com/linxumoney/wisdom-council)** - "智者议会" — 7 top thinkers debate your questions simultaneously. Buffett × Munger × Inamori × Lynch × Naval × Dalio × Thiel. `multi-persona-debate` `Chinese` `License N/A`
  - Distilled personas: Warren Buffett, Charlie Munger, Kazuo Inamori, Peter Lynch, Naval Ravikant, Ray Dalio, Peter Thiel
  - Highlights: Novel multi-perspective debate format with moderator summarizing disagreements. Great for investment and business decisions.

- **[alchaincyf/nuwa-skill](https://github.com/alchaincyf/nuwa-skill)** (Multiple thinker personas) - Feynman, Naval, Munger, Taleb, Paul Graham, Karpathy, Ilya Sutskever distilled via nuwa-skill. `cognitive-framework` `Chinese/English` `MIT`
  - Distilled personas: Feynman, Naval, Munger, Taleb, Paul Graham, Karpathy, Ilya Sutskever
  - Highlights: Each persona as independent installable skill repo. Triple validation ensures authenticity.

---

## 🎭 Other Personas

- **[cantian-ai/bazi-persona-skill](https://github.com/cantian-ai/bazi-persona-skill)** - "八字人格" — Generate persona from birth date using Chinese astrology (Bazi). Zero data needed. `bazi-astrology` `Chinese` `License N/A`
  - Distilled persona: Anyone (based on birth date)
  - Highlights: Zero-data cold start — only needs name and birthday. Supports "cheat mode" for switching analysis perspectives. Dynamic personality that changes over time.

- **Lei Jun Speech Prompt** ([wwsun.github.io](https://wwsun.github.io/prompts/leijun-speech-prompt)) - Single prompt capturing Lei Jun's speech DNA. `prompt-engineering` `Chinese` `N/A`
  - Distilled persona: Lei Jun (speech style)
  - Highlights: Precise expression DNA extraction — "civilian-rooted tech believer", "anti-elite pragmatism", "absolute long-termism with decisive action".

---

## 📋 Awesome Lists & Collections

Other curated lists in the persona distillation space:

- **[ab18108289/awesome-persona-skills](https://github.com/ab18108289/awesome-persona-skills)** - The most comprehensive Chinese persona skill directory. 54+ entries.
- **[tmstack/awesome-persona-skills](https://github.com/tmstack/awesome-persona-skills)** - Index of colleague/boss/ex/self/immortal/nuwa skills.
- **[xixu-me/awesome-persona-distill-skills](https://github.com/xixu-me/awesome-persona-distill-skills)** - Curated list of Agent Skills centered on people, relationships, and methodological perspectives.
- **[kou35/Awesome-social-skill](https://github.com/kou35/Awesome-social-skill)** - Collection of people and relationship AI Skills.

---

## 📊 Methodology Comparison

| Dimension | Cognitive Framework | Chat-based | Universal Framework | Methodology Extraction | Multi-persona Debate |
|---|---|---|---|---|---|
| **Representative** | nuwa-skill | colleague-skill | anyone-skill / immortal-skill | skill-from-masters | wisdom-council |
| **Data Source** | Public materials | Private chat logs | Any source | Web search + DB | Pre-built personas |
| **Extraction Depth** | Deep (5-7 layers) | Medium (work style + communication) | Deep (4-7 dimensions) | Methodology-focused | Philosophical principles |
| **Quality Assurance** | Triple validation | Community feedback | Evidence grading L1-L4 | Cross-validation | Manual tuning |
| **Ethics Check** | ❌ | ❌ | ✅ | ❌ | ❌ |
| **Evolvability** | ✅ (darwin-skill) | ❌ | ✅ (Phase 7 Evolve) | ❌ | ❌ |
| **Best For** | Public figures | Personal relationships | Any person | Domain expertise | Decision-making debates |
| **Effort Required** | Auto (minutes) | Manual data prep | Semi-auto | Auto | Ready to use |

👉 **[Full methodology deep-dive →](methodology/comparison.md)**

---

## 🛠 Tools & Resources

- **[Claude Code](https://docs.anthropic.com/en/docs/claude-code)** - Primary runtime for .skill files
- **[OpenClaw](https://github.com/nicepkg/openclaw)** - Open-source AI agent platform that can run persona skills
- **[skills.sh](https://skills.sh)** - Skill marketplace and discovery platform
- **[AgentSkills.io](https://agentskills.io)** - Agent skills standard and ecosystem
- **[Bloome](https://www.bloome.im)** - Multi-agent collaboration platform for persona skills

👉 **[Full tools list →](resources/tools.md)**

---

## 🤝 Contributing

We welcome contributions! Please see our **[Contributing Guide](CONTRIBUTING.md)** for:

- How to submit a new project (PR template)
- Inclusion criteria
- License requirements

---

## Star History

If you find this list useful, please ⭐ star this repo!

---

## License

This repository's index content is licensed under the [MIT License](LICENSE).

> **Note**: Each listed project has its own license. Please check individual project repositories for their specific terms.
