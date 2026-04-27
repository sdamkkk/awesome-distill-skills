# Tools & Resources

> Platforms, tools, and resources for creating and running persona distillation skills.

[← Back to README](../README.md)

---

## Skill Runtimes

Platforms where you can run persona distillation skills:

| Tool | Description | URL |
|---|---|---|
| **Claude Code** | Anthropic's AI coding agent. Primary runtime for .skill files. | [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code) |
| **OpenClaw** | Open-source AI agent platform that can load and run persona skills. | [github.com/nicepkg/openclaw](https://github.com/nicepkg/openclaw) |
| **Bloome** | Multi-agent collaboration platform — let multiple personas work together in one conversation. | [bloome.im](https://www.bloome.im) |

---

## Skill Marketplaces & Discovery

Where to find and share persona skills:

| Platform | Description | URL |
|---|---|---|
| **skills.sh** | Skill marketplace and discovery platform for Claude Code skills. | [skills.sh](https://skills.sh) |
| **AgentSkills.io** | Agent skills standard and ecosystem. | [agentskills.io](https://agentskills.io) |

---

## Skill Installation

Most skills can be installed with a single command:

```bash
# Install via npx (most common)
npx skills add author/skill-name

# Or clone directly
git clone https://github.com/author/skill-name ~/.claude/skills/skill-name
```

---

## Data Export Tools

For chat-based distillation, you may need to export data from messaging platforms:

| Platform | Export Method |
|---|---|
| **WeChat** | Use backup tools or manual export |
| **iMessage** | macOS Messages app → File > Save as |
| **WhatsApp** | In-app: Settings > Chats > Export Chat |
| **Telegram** | Desktop: Settings > Advanced > Export data |
| **Slack** | Workspace admin: Settings > Import/Export |
| **Discord** | Third-party tools (DiscordChatExporter) |
| **Feishu (飞书)** | Admin console export |
| **DingTalk (钉钉)** | Chat history export |

---

## Research Tools

For cognitive framework distillation, these tools help with research:

| Tool | Use Case |
|---|---|
| **Perplexity AI** | Quick research on public figures |
| **Google Scholar** | Academic papers by or about the person |
| **YouTube transcripts** | Extract text from interviews and talks |
| **Podcast transcription** | Whisper, Otter.ai for audio → text |
| **Archive.org Wayback Machine** | Historical versions of websites and posts |
| **Twitter/X Advanced Search** | Find specific posts by date and keyword |

---

## Quality Validation

Tools for testing the quality of generated skills:

| Approach | How |
|---|---|
| **A/B Testing** | Compare skill output with real quotes |
| **darwin-skill** | nuwa-skill's auto-evolution companion |
| **Community review** | Share on Discord/GitHub for feedback |
| **Known-answer test** | Ask questions you know the answer to |

---

## Standards & Specifications

| Standard | Description | URL |
|---|---|---|
| **OpenPersona** | Open standard for persona description (persona.json + state.json + soul/injection.md) | Part of anyone-skill |
| **OpenClaw Soul Spec** | Soul specification for AI agents | Part of OpenClaw |
| **AgentSkills Standard** | Standard for portable AI skills | [agentskills.io](https://agentskills.io) |

---

## Learning Resources

### Articles
- [从"赛博前任"到"数字老板"：GitHub 爆火的 Person.Skill 背后](https://cloud.tencent.com/developer/article/2655883) — Deep architectural analysis of the persona skill movement
- [你能被装进一个文件里吗？——7 万人把同事"蒸馏"成了 AI](https://www.cnblogs.com/wmyskxz/p/19854791) — Popular science article on the distillation trend
- [nuwa-skill: Turning "distilling a person" from an idea into an engineering problem](https://www.knightli.com/en/2026/04/22/nuwa-skill-distill-how-someone-thinks/) — English analysis of nuwa-skill's methodology

### Communities
- **colleague-skill Discord** — [discord.gg/aRjmJBdK](https://discord.gg/aRjmJBdK) — Active community for dot-skill
- **colleague-skill WeChat Groups** — Multiple groups (check the project README for latest QR codes)

---

## Related Projects (Non-distillation)

Projects that are related but don't focus on distilling specific people:

| Project | Description |
|---|---|
| **Character.ai** | Commercial platform for AI character creation |
| **SillyTavern** | Open-source frontend for AI roleplay |
| **TavernAI** | Another AI character interaction platform |

> Note: These are not persona distillation tools — they focus on roleplay rather than cognitive extraction.

---

[← Back to README](../README.md)
