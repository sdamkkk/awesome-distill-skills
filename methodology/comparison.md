# Methodology Comparison: Persona Distillation Approaches

> A deep dive into the different approaches to distilling human thinking patterns into AI skills.

[← Back to README](../README.md)

---

## Overview

The persona distillation space has evolved rapidly in 2026. What started as simple system prompts ("act like Elon Musk") has grown into sophisticated multi-phase pipelines with research, validation, and evolution mechanisms.

This document compares 5 major approaches:

1. **Pure Prompt Engineering** — Manual prompt crafting
2. **Cognitive Framework Extraction** — Systematic mental model mining
3. **Chat-based Distillation** — Private data → persona
4. **RAG + Vector Retrieval** — Retrieval-augmented persona
5. **Fine-tuning** — Model weight modification

Plus a bonus section on our hybrid approach.

---

## 1. Pure Prompt Engineering

**Representative projects**: Panmax/leijun-skill, wemamawe/ai-persona-skills, wisdom-council

### How it works
Write a detailed system prompt that describes the persona's characteristics, speaking style, key beliefs, and response patterns.

### Typical structure
```
You are [Person X]. You think in terms of [mental models].
Your speaking style is [characteristics].
When asked about [topic], you always [pattern].
```

### Strengths
| Aspect | Rating | Notes |
|---|---|---|
| Speed to create | ⭐⭐⭐⭐⭐ | Minutes to hours |
| Ease of use | ⭐⭐⭐⭐⭐ | No tools needed |
| Portability | ⭐⭐⭐⭐⭐ | Works in any LLM |
| Maintenance | ⭐⭐⭐⭐ | Easy to update |

### Weaknesses
| Aspect | Rating | Notes |
|---|---|---|
| Depth of persona | ⭐⭐ | Surface-level mimicry |
| Authenticity | ⭐⭐ | Often regurgitates quotes |
| Consistency | ⭐⭐⭐ | May break character |
| Scalability | ⭐⭐ | Manual effort per persona |

### When to use
- Quick prototyping
- Simple personas that don't need deep accuracy
- When you need to run in any LLM without infrastructure

---

## 2. Cognitive Framework Extraction

**Representative projects**: nuwa-skill, zhang-yiming-skill

### How it works
Systematically research a person across multiple dimensions, extract their mental models and decision heuristics, validate through cross-referencing, and compile into a structured skill.

### nuwa-skill's 5-layer extraction
```
Layer 1: Expression DNA (how they talk)
    ↓
Layer 2: Mental Models (how they think)
    ↓
Layer 3: Decision Heuristics (how they judge)
    ↓
Layer 4: Anti-Patterns (what they won't do)
    ↓
Layer 5: Honesty Boundaries (what they can't know)
```

### nuwa-skill's 6-way research pipeline
1. **Books & writings** — Primary authored works
2. **Podcasts & interviews** — Spontaneous spoken thoughts
3. **Social media** — Real-time reactions and hot takes
4. **Critics' perspective** — What opponents say
5. **Decision records** — Actual choices they made
6. **Life timeline** — How thinking evolved over time

### Triple validation
A mental model is valid only if it:
- ✅ Appears across 2+ domains (not a one-off comment)
- ✅ Can predict stance on new questions (has predictive power)
- ✅ Is not shared by all smart people (is exclusionary)

### Strengths
| Aspect | Rating | Notes |
|---|---|---|
| Depth of persona | ⭐⭐⭐⭐⭐ | Captures cognitive OS |
| Authenticity | ⭐⭐⭐⭐⭐ | Uses real mental models |
| Novel responses | ⭐⭐⭐⭐⭐ | Can address new topics authentically |
| Transparency | ⭐⭐⭐⭐ | Research process is traceable |

### Weaknesses
| Aspect | Rating | Notes |
|---|---|---|
| Speed to create | ⭐⭐⭐ | Automated but needs research time |
| Private personas | ⭐⭐ | Needs public materials |
| Token cost | ⭐⭐⭐ | Multi-step pipeline |
| Emotional depth | ⭐⭐⭐ | Better at thinking than feeling |

### When to use
- Public figures with extensive public materials
- When you need the persona to handle novel questions authentically
- When quality matters more than speed

---

## 3. Chat-based Distillation

**Representative projects**: colleague-skill (dot-skill), ex-skill, immortal-skill

### How it works
Feed the AI private data sources (chat logs, messages, documents, photos) and extract personality patterns, communication style, knowledge, and relationship dynamics.

### ex-skill's 6-layer personality extraction
```
Layer 1: Core Rules (fundamental behavioral patterns)
Layer 2: Identity (self-concept and values)
Layer 3: Expression (speaking style, vocabulary, emoji usage)
Layer 4: Emotional Patterns (when they get excited, withdrawn, angry)
Layer 5: Conflict & Boundaries (how they argue, what they avoid)
Layer 6: Triggers (what specifically activates reactions)
```

### Data sources typically supported
- WeChat / QQ messages
- Feishu / DingTalk documents
- Email archives
- iMessage exports
- WhatsApp / Telegram exports
- Social media posts
- Photos and screenshots

### Strengths
| Aspect | Rating | Notes |
|---|---|---|
| Emotional accuracy | ⭐⭐⭐⭐⭐ | Captures real interaction patterns |
| Personal knowledge | ⭐⭐⭐⭐⭐ | Remembers shared experiences |
| Communication style | ⭐⭐⭐⭐⭐ | Exact vocabulary and emoji patterns |
| Intimacy | ⭐⭐⭐⭐⭐ | Feels like the real person |

### Weaknesses
| Aspect | Rating | Notes |
|---|---|---|
| Ethics / privacy | ⭐ | Major consent concerns |
| Data preparation | ⭐⭐ | Requires manual export and cleanup |
| Thinking depth | ⭐⭐⭐ | Captures style more than cognition |
| Generalization | ⭐⭐ | Only works for specific relationships |

### When to use
- Personal relationships (with consent!)
- Knowledge preservation from departing team members
- Self-distillation for personal reflection

---

## 4. RAG + Vector Retrieval

**Representative projects**: Some implementations within anyone-skill, various custom builds

### How it works
Index a corpus of the person's materials into a vector database, and retrieve relevant passages at query time to ground the persona's responses in actual source material.

### Typical architecture
```
Corpus (books, talks, articles)
    ↓ Embedding
Vector Database
    ↓ Semantic Search (at query time)
Retrieved Passages + System Prompt
    ↓ LLM Generation
Persona Response (grounded in real quotes)
```

### Strengths
| Aspect | Rating | Notes |
|---|---|---|
| Factual accuracy | ⭐⭐⭐⭐⭐ | Grounded in actual materials |
| Scalability | ⭐⭐⭐⭐ | Easy to add new materials |
| Traceability | ⭐⭐⭐⭐⭐ | Can cite sources |
| Updatability | ⭐⭐⭐⭐ | Add new docs without rebuild |

### Weaknesses
| Aspect | Rating | Notes |
|---|---|---|
| Infrastructure | ⭐⭐ | Needs vector DB setup |
| Novel responses | ⭐⭐⭐ | Limited to existing material |
| Persona coherence | ⭐⭐⭐ | May mix different periods |
| Cost | ⭐⭐ | Embedding + retrieval + generation |

### When to use
- When factual grounding is critical
- Large corpus of materials available
- When you need citation for every claim

---

## 5. Fine-tuning

**Representative projects**: Rare in the open-source persona space (high barrier)

### How it works
Create a training dataset of the person's writing/speaking and fine-tune an LLM to internalize their patterns at the weight level.

### Strengths
| Aspect | Rating | Notes |
|---|---|---|
| Naturalness | ⭐⭐⭐⭐⭐ | Deeply embedded in weights |
| Consistency | ⭐⭐⭐⭐⭐ | Won't break character |
| Speed at inference | ⭐⭐⭐⭐⭐ | No retrieval overhead |
| Expression accuracy | ⭐⭐⭐⭐⭐ | Truly sounds like the person |

### Weaknesses
| Aspect | Rating | Notes |
|---|---|---|
| Cost | ⭐ | Expensive training |
| Data requirements | ⭐ | Needs large clean dataset |
| Updatability | ⭐ | Must retrain to update |
| Portability | ⭐ | Tied to specific model |
| Accessibility | ⭐ | Requires ML expertise |

### When to use
- Production applications requiring maximum consistency
- When you have abundant training data and budget
- Long-term deployments that justify training cost

---

## 6. Hybrid Approach (Our Method)

**Representative projects**: leijun-distill-skill (WIP)

### How it works
Combine the best of each approach:

```
Phase 1: Multi-source Corpus Collection
    Books, speeches, interviews, social media, critic perspectives
        ↓
Phase 2: Batch Refinement
    Process in batches → Extract patterns → Cross-validate
        ↓
Phase 3: Structured Knowledge Cards
    Mental models, decision heuristics, expression DNA,
    anti-patterns, honesty boundaries (with evidence grading)
        ↓
Phase 4: Skill Generation
    Compile into SKILL.md with transparent research trail
        ↓
Phase 5: Quality Validation
    3 known questions + 1 edge case + style consistency check
```

### Design principles
1. **Transparent research** — All raw materials and reasoning published
2. **Preserve contradictions** — Real people have contradictions; don't flatten them
3. **Evidence grading** — L1 (direct quote) → L2 (repeated) → L3 (inferred) → L4 (inspired)
4. **Honesty boundaries** — Explicitly state what the skill doesn't know
5. **Anti-patterns** — Document what the person would NOT do

---

## Side-by-Side Comparison

| Dimension | Prompt Engineering | Cognitive Framework | Chat-based | RAG | Fine-tuning | Hybrid |
|---|---|---|---|---|---|---|
| **Setup Time** | Minutes | Hours | Hours | Days | Weeks | Days |
| **Thinking Depth** | ⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Expression Accuracy** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| **Novel Q Handling** | ⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Factual Grounding** | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **Infrastructure** | None | None | None | Vector DB | GPU | None |
| **Cost** | Free | Low | Free | Medium | High | Low |
| **Portability** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ | ⭐ | ⭐⭐⭐⭐ |
| **Ethics Risk** | Low | Low | High | Low | Medium | Low |
| **Best For** | Quick prototypes | Public figures | Personal relations | Large corpus | Production | Deep distillation |

---

## Recommendation Matrix

| Your scenario | Recommended approach | Why |
|---|---|---|
| "I want to quickly try distilling someone" | Prompt Engineering | Fast, zero setup |
| "I need a deep, authentic public figure" | Cognitive Framework (nuwa-skill) | Best depth + auto pipeline |
| "I want to preserve a departing colleague" | Chat-based (colleague-skill) | Uses available work data |
| "I want factual accuracy with citations" | RAG | Grounded in source material |
| "I need production-grade consistency" | Fine-tuning | Deepest integration |
| "I want the best of all worlds" | Hybrid | Combines strengths |

---

[← Back to README](../README.md) | [Best Practices →](best-practices.md)
