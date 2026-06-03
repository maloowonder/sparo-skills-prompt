<div align="center">

# 🔥 GRILL-ME 系列

**让你的方案无处藏身 —— 8 款毫不留情的 AI 审查工具**

[English](./README.en.md) · ·

*战略 · 产品 · 运营 · 投资 · 学术 · 内容 · 审计*

从通用方案讨论到七大专业领域的深度审查，覆盖商业决策全场景。

</div>

---

## 这是什么？

**GRILL-ME** 是一套为 AI 助手设计的「毫不留情审查」技能/提示词集合。

传统 AI 回复往往是礼貌的、模糊的、甚至过度肯定的。这套工具的核心理念是 **反转 AI 的默认立场** ——让 AI 从「讨好型助手」变成「苛刻的审查官」，按照各领域的专业标准，对方案进行逐层拆解、追问到底。

每一条 GRILL-ME 规则都严格执行：

| 规则 | 说明 |
|------|------|
| ⚡ **一次一问** | 等你答完，再问下一个。绝不一次抛出多个问题让你无所适从 |
| 🎯 **必附推荐决策** | 每个问题附带【推荐答案 + 理由 + Trade-off】——不是把球踢给你，而是告诉你这个节点上通常怎么选、选错会怎样 |
| 🔢 **具体到数字** | 拒绝「你有数据支持吗」这类笼统追问。改为「你的 7 日留存预期提升多少？如果只提升 0.5%，开发量还值得吗？」 |
| 🧠 **常识优先** | 能通过行业基准/方法论常识推断的问题，直接指出漏洞，不浪费时间问已知信息 |
| 🚫 **禁区明确** | 不讨论排版配色、不发散脑洞、不给模糊安慰 —— 唯一目标是把方案审到无懈可击 |

## 八大审查领域

| Skill | 领域 | 核心审查轴 | 默认立场 | 对标角色 |
|:------|:-----|:-----------|:---------|:---------|
| [grill-me](skills/grill-me/grill-me/) | 🔧 通用 | 架构 / 设计 / 技术决策 | 中性质疑 | 资深工程师 |
| [consulting-grill-me](skills/grill-me/consulting-grill-me/) | 🏢 战略管理 | 底层假设 · 价值创造逻辑 · 实施路线图 · 资源约束 | 质疑乐观假设 | MBB 合伙人 |
| [pm-grill-me](skills/grill-me/pm-grill-me/) | 📱 产品设计 | 用户价值 · 商业模式 · 优先级 ROI · 数据闭环 | 质疑伪需求 | 资深 CPO |
| [ops-grill-me](skills/grill-me/ops-grill-me/) | 📈 运营增长 | 北极星指标 · 单位经济模型 · 漏斗节点 · 风险熔断 | 质疑虚高 GMV | COO / 增长负责人 |
| [investor-grill-me](skills/grill-me/investor-grill-me/) | 💰 风险投资 | Unit Economics · TAM/SAM/SOM · 护城河 · 估值 · 退出 | **证伪主义** | VC/PE 合伙人 |
| [research-grill-me](skills/grill-me/research-grill-me/) | 🔬 学术研究 | Research Gap · 假设推导 · 方法适切性 · 内生性 · 伦理 | **可证伪性** | 顶刊匿名审稿人 |
| [creator-grill-me](skills/grill-me/creator-grill-me/) | 🎬 内容创作 | 3秒钩子 · 信息密度 · 人设构建 · 变现闭环 | 算法逻辑反推 | MCN 内容总监 |
| [audit-grill-me](skills/grill-me/audit-grill-me/) | 📋 审计风控 | 控制设计有效性 · 风险敞口 · 样本代表性 · 缺陷整改 | **舞弊三角** | 四大合伙人 |

## 适合谁？

- **创业者 / 产品经理**：用 `pm-grill-me` 和 `ops-grill-me` 在内部评审前自我压测，减少被投资人/老板当场追问的尴尬
- **投资人 / 分析师**：用 `investor-grill-me` 对标 BP 进行系统化拆解，避免被漂亮的故事迷惑
- **咨询顾问 / 战略规划师**：用 `consulting-grill-me` 检验方案底层假设，确保交付给客户之前方案经得起拷问
- **研究生 / 研究人员**：用 `research-grill-me` 在投稿前模拟 Reviewer 2 的攻击，提前补上方法论漏洞
- **内容创作者 / MCN**：用 `creator-grill-me` 用算法逻辑审查选题，避免「看起来好但数据差」的内容
- **内审 / 风控 / 合规**：用 `audit-grill-me` 从舞弊三角视角排查内控盲区
- **任何需要「第二意见」的人**：用 `grill-me` 做通用的方案压力测试

## 仓库结构

```
sparo-skills-prompt/
├── README.md                     # 中文说明（本文件）
├── README.en.md                  # English README
├── LICENSE                       # MIT License
├── skills/                       # WorkBuddy Skill 格式
│   └── grill-me/
│       ├── grill-me/
│       │   └── SKILL.md          # 通用审查
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
└── prompt/                       # 通用 Prompt 格式（适配任何 AI）
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

> **注意**：`prompt/` 目录仅包含 7 个专业领域 Prompt，通用审查请直接使用 `skills/grill-me/grill-me/SKILL.md`。

## 使用方式

### 方式一：WorkBuddy 用户（推荐）

将 `skills/` 目录下对应的 SKILL.md 安装到你的 WorkBuddy 环境：

```bash
# 安装到用户级（所有项目可用）
cp -r skills/grill-me/pm-grill-me ~/.workbuddy/skills/
```

安装后直接输入斜杠命令触发：

```
/pm-grill-me
```

或用自然语言触发：

```
「帮我压测一下这个产品方案」
「审查我的运营策略」
```

### 方式二：通用 Prompt（适配任何 AI 工具）

将 `prompt/grill-me/` 目录下的 `prompt.md` 文件内容直接粘贴到 ChatGPT、Claude、Gemini 等任意 AI 对话工具中即可使用。每条 Prompt 都是自包含的——复制、粘贴、贴出你的方案，开始接受审查。

### 方式三：API 集成

将 Prompt 作为 System Prompt 注入到你的 AI 应用中：

```python
system_prompt = open("prompt/grill-me/pm-grill-me/prompt.md").read()
# 传入你的 LLM API
```

## 设计哲学

### 为什么需要「GRILL」？

大多数 AI 助手的默认行为模式是 **肯定优先** ——用户说什么，AI 倾向于附和或温和地补充。这在日常对话中没问题，但在严肃的方案审查场景中是危险的。

GRILL-ME 系列的核心设计原则是 **立场反转**：

| 领域 | AI 默认立场 | GRILL-ME 立场 |
|------|------------|---------------|
| 投资 | 「这个赛道有机会」 | **证伪主义**——默认不值得投，直到你证明它值得 |
| 学术 | 「这个方向挺有意思」 | **可证伪性**——你的假设能不能被证伪？不能就不是科学 |
| 审计 | 「这个控制总体还行」 | **舞弊三角**——默认每个节点都可能被绕开 |
| 运营 | 「活动思路不错」 | **ROI 怀疑**——你预测的 GMV 有多少是注水 |
| 产品 | 「这个功能用户会喜欢」 | **伪需求猎手**——你确信这不是 XY Problem |

### 从「填鸭式审查」到「苏格拉底式追问」

传统审查清单（Checklist）的问题在于：它只能检查你是否「填了所有格子」，不能检查你「填得对不对」。

GRILL-ME 采用 **苏格拉底式追问** ——沿着逻辑树/依赖树逐层推进，每个问题都建立在上一层的回答之上。这意味着：
- 你不能跳过薄弱环节
- 你不能藏在笼统描述里
- 每一层的答案都会成为下一层的追问依据

## 贡献指南

欢迎提交新的领域审查 Skill！请遵循以下规范：

1. **一个 Skill 对应一个专业领域**，不要合并
2. **必须有明确的默认立场**（证伪/可证伪/舞弊三角/算法反推……），不能是「中立客观」
3. **提问规则五条铁律**必须完整保留（一次一问、必附推荐、具体到数字、常识优先、禁区明确）
4. **必须有结束条件**——明确多少条标准满足后才能宣布审查通过
5. **Prompt 文件必须是自包含的**——不依赖外部工具或特定 AI 平台

提交 PR 时请同时提供：
- `skills/grill-me/<name>/SKILL.md`（WorkBuddy 格式）
- `prompt/grill-me/<name>/prompt.md`（通用 Prompt 格式）

## 许可证

[MIT License](./LICENSE)

---

<div align="center">

**让你的每一个决策都经得起拷问。**

</div>
