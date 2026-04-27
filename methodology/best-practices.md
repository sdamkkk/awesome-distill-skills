# Best Practices for Persona Distillation

> Lessons learned from studying 15+ persona distillation projects.

[← Back to README](../README.md) | [← Methodology Comparison](comparison.md)

---

## 1. Corpus Collection Strategy

### Multi-source is non-negotiable

Never rely on a single source. Different materials reveal different facets:

| Source Type | What it reveals | Example |
|---|---|---|
| **Books / writings** | Deliberate, refined thinking | Lei Jun's autobiography |
| **Interviews / podcasts** | Spontaneous reasoning | Lex Fridman interviews |
| **Social media** | Real-time reactions, hot takes | Twitter/Weibo posts |
| **Speeches / keynotes** | Public persona, persuasion style | Apple keynotes |
| **Decision records** | Actual choices under pressure | M&A decisions, pivots |
| **Critics' perspective** | Blind spots, contradictions | Competitor critiques |
| **Life timeline** | How thinking evolved | Career transitions |

### The nuwa-skill 6-way approach

The gold standard (from nuwa-skill) is to research across 6 parallel tracks:

```
1. 📚 Primary works (books, papers, blog posts)
2. 🎙️ Spoken word (podcasts, interviews, speeches)
3. 📱 Social media (tweets, posts, comments)
4. 👁️ Third-party perspective (critics, biographers, competitors)
5. 📊 Decision records (actual choices and their outcomes)
6. 📅 Life timeline (chronological evolution)
```

### Quantity guidelines

From studying zhang-yiming-skill (the most transparent example):
- **32+ interview fragments** for a single person
- **12+ major decision cases**
- **6 research files, 1380+ lines** of raw notes
- This produces a high-quality, defensible skill

### Tips
- ✅ Prioritize primary sources over secondary commentary
- ✅ Include materials from different time periods (people evolve)
- ✅ Seek out **contradictions** — they make the persona real
- ❌ Don't only use positive/admiring sources
- ❌ Don't rely on Wikipedia summaries

---

## 2. Extraction Dimensions

### The 5-layer cognitive model (nuwa-skill)

The most proven extraction framework:

| Layer | What to extract | Example (Lei Jun) |
|---|---|---|
| **Expression DNA** | Vocabulary, sentence patterns, rhythm, forbidden words, confidence levels | Humble tone, data-driven arguments, "Are you OK?" |
| **Mental Models** | Core thinking frameworks (3-7) | Extreme value-for-money, riding the wave, internet thinking 7-word formula |
| **Decision Heuristics** | How they make choices (5-10) | "If it doesn't benefit 80% of users, remove it" |
| **Anti-Patterns** | What they would NEVER do | Never compete on premium alone without volume |
| **Honesty Boundaries** | What the skill can't know | Doesn't know about post-2024 events, can't give legal advice |

### Evidence grading (from OpenPersona/anyone-skill)

Every extracted insight should be tagged with confidence:

| Level | Description | Example |
|---|---|---|
| **L1 - Direct Quote** | Person said exactly this | "站在风口上，猪都能飞起来" |
| **L2 - Repeated Pattern** | Expressed the same idea multiple times | Value-for-money mentioned in 15+ speeches |
| **L3 - Inferred** | Logically derived from actions/context | Xiaomi's pricing strategy implies volume-over-margin thinking |
| **L4 - Inspired** | Loosely inspired, not directly attributable | General industry analysis in Lei Jun's style |

### The triple validation test (nuwa-skill)

A mental model is only valid if it passes 3 checks:

1. **Cross-domain**: Appears in 2+ different contexts (not a one-off comment)
2. **Predictive**: Can predict the person's stance on a new question
3. **Exclusionary**: Not something all smart people would say (uniquely theirs)

---

## 3. Quality Validation

### The 4-question test

After generating a skill, validate with:

1. **3 known questions** — Ask questions you know how the person answered. Does the skill match?
2. **1 edge case** — Ask something outside their usual domain. Does the reasoning feel authentic?
3. **Style check** — Read the output aloud. Does it sound like the person or a Wikipedia article?

### Common failure modes

| Failure | Symptom | Fix |
|---|---|---|
| **Quote machine** | Only regurgitates famous quotes | Focus on mental models, not catchphrases |
| **Wikipedia voice** | Sounds like an encyclopedia entry | Add expression DNA layer |
| **Flattery trap** | Always agrees with the user | Add anti-patterns and disagreement capacity |
| **Time collapse** | Mixes 2010 and 2024 thinking | Add temporal awareness |
| **Shallow mimicry** | Copies surface style without reasoning | Deepen mental model extraction |

### A/B comparison

The ultimate test: show the skill's output alongside a real quote to someone familiar with the person. Can they tell which is which? If the skill's output is indistinguishable (or at least in the same ballpark), you've succeeded.

---

## 4. Skill File Structure

### Recommended SKILL.md structure

Based on patterns from the best projects:

```markdown
# [Person Name] Skill

## Identity
Who this person is, core identity statement.

## Mental Models
### Model 1: [Name]
- Description
- When to apply
- Example application

### Model 2: [Name]
...

## Decision Heuristics
1. [Heuristic with context]
2. [Heuristic with context]
...

## Expression DNA
- Tone: [description]
- Vocabulary: [characteristic words/phrases]
- Sentence patterns: [structures they favor]
- Forbidden: [things they'd never say]

## Anti-Patterns
- [What this person would NOT do]
- [Beliefs they'd reject]

## Honesty Boundaries
- [What this skill cannot answer]
- [Temporal limitations]
- [Domain limitations]

## References
- [Source 1] — [how it was used]
- [Source 2] — [how it was used]
```

### Key principles
- ✅ Mental models > catchphrases
- ✅ Include anti-patterns (what they wouldn't do)
- ✅ State honesty boundaries explicitly
- ✅ Link to research sources for transparency
- ✅ Keep expression DNA specific and measurable

---

## 5. Preserving Contradictions

### Why contradictions matter

Real people are inconsistent. The best distillation skills preserve this:

| Person | Contradiction | Why it matters |
|---|---|---|
| Zhang Yiming | "Delayed gratification" vs built Douyin (instant gratification) | Shows strategic vs product thinking |
| Lei Jun | "Extreme value-for-money" vs Xiaomi Ultra premium line | Shows evolution of thinking |
| Elon Musk | "First principles" vs often using analogies | Shows pragmatism |

### How to handle contradictions
1. **Document both sides** — Don't flatten the person into consistency
2. **Add temporal context** — "In 2015 he believed X, by 2022 he shifted to Y"
3. **Explain the tension** — "This contradiction reflects the gap between his philosophy and business reality"
4. **Let the skill navigate** — When asked, the skill should acknowledge the tension rather than pretend it doesn't exist

---

## 6. Ethical Considerations

### For public figures
- ✅ Use only publicly available materials
- ✅ Add disclaimer that the skill is a model, not the actual person
- ✅ State limitations clearly
- ❌ Don't claim to represent the person's actual current views
- ❌ Don't generate content that could damage the person's reputation

### For private individuals
- ✅ Obtain explicit consent from the person being distilled
- ✅ Allow the distilled person to review and veto the skill
- ✅ Include a clear privacy notice
- ❌ Don't distill someone without their knowledge
- ❌ Don't share private persona skills publicly without consent

### General principles
- Always include a disclaimer at the top of the skill
- Make it clear this is an AI interpretation, not the real person
- Respect intellectual property — quote and attribute properly
- Consider what the distilled person would think of the skill

---

## 7. Common Pitfalls

| Pitfall | Description | How to avoid |
|---|---|---|
| **Hagiography** | Making the person seem perfect | Include critics' perspective and anti-patterns |
| **Recency bias** | Over-weighting recent materials | Sample across the full timeline |
| **Language bias** | Missing non-English/non-Chinese sources | Search in the person's native language |
| **Selection bias** | Only using materials that confirm a narrative | Include contradictory evidence |
| **Style over substance** | Nailing the voice but missing the thinking | Prioritize mental models over expression DNA |
| **Context collapse** | Applying advice from one domain to all domains | Tag mental models with applicable contexts |
| **Stale persona** | Not accounting for how the person evolved | Include temporal markers |
| **Echo chamber** | Only using fan-produced materials | Include critical and opposing perspectives |

---

## 8. Evolution and Maintenance

### Keep skills alive

A distilled skill should evolve as new information becomes available:

1. **Watch for new materials** — New interviews, speeches, decisions
2. **Validate periodically** — Does the skill still hold up against new data?
3. **Version control** — Track changes to the skill over time
4. **Community feedback** — Let users report inaccuracies
5. **Auto-evolution** — Tools like nuwa-skill's darwin-skill can help

### The darwin-skill approach

nuwa-skill includes a companion "darwin-skill" that:
- Automatically reviews and optimizes generated skills
- Tests for consistency and depth
- Suggests improvements based on new research
- This is the gold standard for skill evolution

---

## Summary Checklist

Before publishing a persona distillation skill:

- [ ] Collected from 3+ different source types
- [ ] Extracted 3-7 mental models with evidence
- [ ] Included 5-10 decision heuristics
- [ ] Documented expression DNA (specific, not generic)
- [ ] Listed anti-patterns (what the person wouldn't do)
- [ ] Stated honesty boundaries
- [ ] Preserved known contradictions
- [ ] Validated with 3 known + 1 edge case questions
- [ ] Added disclaimer and ethical notice
- [ ] Linked to research sources
- [ ] Tagged evidence with confidence levels (L1-L4)

---

[← Back to README](../README.md) | [← Methodology Comparison](comparison.md)
