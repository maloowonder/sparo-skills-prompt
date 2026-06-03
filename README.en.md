<div align="center">

# 🔥 GRILL-ME Series

**No Mercy for Flawed Plans — 8 Relentless AI Review Skills**

English · [中文](./README.md)

*Strategy · Product · Operations · Investment · Research · Content · Audit*

From general-purpose review to deep-domain expertise — covering the full spectrum of business decision-making.

</div>

---

## What Is This?

**GRILL-ME** is a collection of "no-mercy review" skills and prompts designed for AI assistants.

The default behavior of most AI assistants is to be polite, vague, and overly affirming. This toolkit **reverses that default stance** — turning AI from a "yes-person" into a "ruthless examiner" that systematically dissects your proposals according to professional standards in each domain.

Every GRILL-ME rule is strictly enforced:

| Rule | Description |
|------|-------------|
| ⚡ **One question at a time** | Wait for your answer before asking the next. Never overwhelm you with multiple questions |
| 🎯 **Mandatory recommendation** | Every question includes a [Recommended Answer + Rationale + Trade-off] — it doesn't just kick the ball back to you |
| 🔢 **Specific to numbers** | No vague "Do you have data?" probes. Instead: "What's your expected 7-day retention lift? If it's only 0.5%, is the dev effort still worth it?" |
| 🧠 **Common sense first** | If a gap can be identified through industry benchmarks or methodological common sense, it's called out directly — no time wasted on knowns |
| 🚫 **Clear boundaries** | No design discussions, no brainstorming rabbit holes, no vague encouragement — the sole objective is to stress-test your plan until it's bulletproof |

## Eight Review Domains

| Skill | Domain | Core Review Axes | Default Stance | Role Model |
|:------|:-------|:-----------------|:---------------|:-----------|
| [grill-me](skills/grill-me/grill-me/) | 🔧 General | Architecture / Design / Tech Decisions | Neutral skepticism | Senior Engineer |
| [consulting-grill-me](skills/grill-me/consulting-grill-me/) | 🏢 Strategy | Underlying Assumptions · Value Creation Logic · Roadmap · Resource Constraints | Challenges optimistic assumptions | MBB Partner |
| [pm-grill-me](skills/grill-me/pm-grill-me/) | 📱 Product | User Value · Business Model · Priority ROI · Data Loop | Challenges phantom requirements | CPO |
| [ops-grill-me](skills/grill-me/ops-grill-me/) | 📈 Operations | North Star · Unit Economics · Funnel Nodes · Circuit Breaker | Challenges inflated GMV | COO / Growth Lead |
| [investor-grill-me](skills/grill-me/investor-grill-me/) | 💰 Investment | Unit Economics · TAM/SAM/SOM · Moat · Valuation · Exit | **Falsificationism** | VC/PE Partner |
| [research-grill-me](skills/grill-me/research-grill-me/) | 🔬 Research | Research Gap · Hypothesis Logic · Methodology Fit · Endogeneity · Ethics | **Falsifiability** | Top-Journal Reviewer |
| [creator-grill-me](skills/grill-me/creator-grill-me/) | 🎬 Content Creation | 3s Hook · Information Density · Persona · Monetization | Algorithm-driven critique | MCN Content Director |
| [audit-grill-me](skills/grill-me/audit-grill-me/) | 📋 Audit & Risk | Control Design · Risk Exposure · Sampling · Remediation Loop | **Fraud Triangle** | Big 4 Partner |

## Who Is This For?

- **Founders / Product Managers**: Use `pm-grill-me` and `ops-grill-me` to stress-test before internal reviews — reduce the awkwardness of being grilled by investors or bosses
- **Investors / Analysts**: Use `investor-grill-me` to systematically dissect pitch decks — avoid being seduced by compelling narratives
- **Consultants / Strategists**: Use `consulting-grill-me` to validate underlying assumptions — ensure your deliverables survive client scrutiny
- **Graduate Students / Researchers**: Use `research-grill-me` to simulate Reviewer 2's attack before submission — patch methodology gaps early
- **Content Creators / MCN Teams**: Use `creator-grill-me` to review topics through algorithm logic — avoid "looks great, performs poorly" content
- **Internal Audit / Risk / Compliance**: Use `audit-grill-me` to scan for control blind spots through the fraud triangle lens
- **Anyone who needs a "second opinion"**: Use `grill-me` for general-purpose plan stress-testing

## Repository Structure

```
sparo-skills-prompt/
├── README.md                     # Chinese documentation
├── README.en.md                  # English documentation (this file)
├── LICENSE                       # MIT License
├── skills/                       # WorkBuddy Skill format
│   └── grill-me/
│       ├── grill-me/
│       │   └── SKILL.md          # General review
│       ├── consulting-grill-me/
│       │   └── SKILL.md
│       ├── pm-grill-me/
│       │   └── SKILL.md
│       ├── ops-grill-me/
│       │   └── SKILL.md
│       ├── investor-grill-me/
│       │   └── SKILL.md
│       ├── research-grill-me/
│       │   └── SKILL.md
│       ├── creator-grill-me/
│       │   └── SKILL.md
│       └── audit-grill-me/
│           └── SKILL.md
└── prompt/                       # Universal Prompt format (works with any AI)
    └── grill-me/
        ├── audit-grill-me/
        │   └── prompt.md
        ├── consulting-grill-me/
        │   └── prompt.md
        ├── creator-grill-me/
        │   └── prompt.md
        ├── investor-grill-me/
        │   └── prompt.md
        ├── ops-grill-me/
        │   └── prompt.md
        ├── pm-grill-me/
        │   └── prompt.md
        └── research-grill-me/
            └── prompt.md
```

> **Note**: The `prompt/` directory only contains 7 domain-specific prompts. For general review, use `skills/grill-me/grill-me/SKILL.md`.

## Usage

### Option 1: WorkBuddy Users (Recommended)

Install the SKILL.md files to your WorkBuddy environment:

```bash
# Install at user level (available in all projects)
cp -r skills/grill-me/pm-grill-me ~/.workbuddy/skills/
```

Trigger with slash commands:

```
/pm-grill-me
```

Or with natural language:

```
"Stress-test this product plan for me"
"Review my growth strategy"
```

### Option 2: Universal Prompts (Any AI Tool)

Copy the contents of any `prompt.md` file from the `prompt/grill-me/` directory and paste it directly into ChatGPT, Claude, Gemini, or any other AI conversation tool. Each prompt is self-contained — copy, paste, submit your plan, and let the grilling begin.

### Option 3: API Integration

Inject prompts as system prompts into your AI applications:

```python
system_prompt = open("prompt/grill-me/pm-grill-me/prompt.md").read()
# Pass to your LLM API
```

## Design Philosophy

### Why "GRILL"?

The default behavior of most AI assistants is **affirmation-first** — whatever the user says, the AI tends to agree or gently supplement. This is fine for casual conversation but dangerous in serious review scenarios.

The core design principle of GRILL-ME is **stance reversal**:

| Domain | AI Default Stance | GRILL-ME Stance |
|--------|-------------------|-----------------|
| Investment | "This sector has potential" | **Falsificationism** — not worth investing until you prove it is |
| Research | "Interesting direction" | **Falsifiability** — can your hypothesis be disproven? If not, it's not science |
| Audit | "Controls look generally fine" | **Fraud Triangle** — every node can potentially be bypassed |
| Operations | "Great campaign concept" | **ROI Skepticism** — how much of your projected GMV is inflated? |
| Product | "Users will love this feature" | **Phantom Requirement Hunter** — are you sure this isn't an XY Problem? |

### From "Checklist Review" to "Socratic Interrogation"

The problem with traditional review checklists is that they only verify whether you've "filled in all the boxes" — not whether you've filled them **correctly**.

GRILL-ME uses **Socratic interrogation** — progressing layer by layer along a logic/dependency tree. Each question builds on the previous answer. This means:
- You can't skip weak links
- You can't hide behind vague descriptions
- Every answer becomes the foundation for the next question

## Contributing

New domain review skills are welcome! Please follow these guidelines:

1. **One Skill per professional domain** — don't merge domains
2. **Must have a clear default stance** (falsification/falsifiability/fraud triangle/algorithm-driven, etc.) — no "neutral and objective"
3. **Five Iron Rules of questioning must be preserved in full** (one at a time, mandatory recommendation, specific numbers, common sense first, clear boundaries)
4. **Must have explicit completion criteria** — a defined number of standards that must all be met before declaring the review passed
5. **Prompt files must be self-contained** — no dependency on external tools or specific AI platforms

When submitting a PR, please provide both:
- `skills/grill-me/<name>/SKILL.md` (WorkBuddy format)
- `prompt/grill-me/<name>/prompt.md` (Universal Prompt format)

## License

[MIT License](./LICENSE)

---

<div align="center">

**Make every decision you make withstand scrutiny.**

</div>
