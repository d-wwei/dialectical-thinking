# Dialectical Thinking | 矛盾论

A cognitive base built on Mao Zedong's *On Contradiction* (《矛盾论》) that shifts AI agent reasoning from seeking correct answers to identifying contradiction networks, locating the principal contradiction, and synthesizing beyond opposition. Works with any LLM agent — Claude, GPT, Gemini, or custom frameworks.

基于毛泽东《矛盾论》构建的认知底座，将 AI agent 的推理方式从"寻找正确答案"转变为"识别矛盾网络、定位主要矛盾、在对立中综合"。适用于任何 LLM agent — Claude、GPT、Gemini 或自定义框架。

---

## What it does | 它做什么

Most AI agents treat problems as optimization puzzles — list the factors, weigh trade-offs, pick the best option. Dialectical Thinking adds a reasoning layer that sees every situation as a network of contradictions, finds the one that matters most, and determines whether to resolve, transform, or let it drive development.

大多数 AI agent 把问题当作优化题——列出因素、权衡利弊、选择最优。矛盾论增加了一个推理层——把每个局面看作矛盾网络，找到最重要的那个矛盾，判断应该化解、转化还是让它推动发展。

### Before (default agent) | 安装前

> "We need both speed and quality in our engineering team."
>
> "Here are 5 best practices to balance speed and quality: automated testing, code reviews, CI/CD, clear acceptance criteria, technical debt budgets..."

### After (with Dialectical Thinking) | 安装后

> "Speed vs quality is a secondary contradiction. Your principal contradiction is that your architecture couples deployment to the entire system — so every change is high-risk, which forces slowness. Decouple deployment (modular boundaries, feature flags), and speed and quality stop being opposed. They were never truly contradictory — they were symptoms of an architectural contradiction."

---

## Core cognitive shift | 核心认知转换

**From**: Find the correct answer
**To**: Identify the contradiction network, locate the principal contradiction, synthesize beyond opposition

从"寻找正确答案"到"识别矛盾网络、定位主要矛盾、在对立之上综合"

---

## How it works | 工作原理

**Six dialectical operations** applied to every reasoning task:

六个辩证操作，应用于每一个推理任务：

| Default mode | Dialectical mode |
|---|---|
| List factors and weigh them 列出因素并权衡 | Map opposing forces as contradictions 将对立力量映射为矛盾 |
| Treat all issues as equal 所有问题同等对待 | Locate the principal contradiction 定位主要矛盾 |
| Seek balance and compromise 寻求平衡与妥协 | Judge nature: reconcile or resolve decisively 判断性质：调和还是决断 |
| Analyze once, then execute 分析一次后执行 | Monitor transformation — re-map when conditions change 监控转化——条件变化时重新定位 |
| Dismiss the opposing view 忽视对立观点 | Steel-man the opposition before synthesizing 综合之前先强化对立面 |
| Apply proven frameworks 套用成熟框架 | Concrete analysis of concrete conditions 具体情况具体分析 |

**Six anti-patterns** that catch fake dialectical reasoning:

六个反模式，捕捉伪辩证推理：

| Anti-pattern 反模式 | Description 描述 |
|---|---|
| Pseudo-synthesis 伪综合 | Appears to combine both sides but actually just picks one 看似综合对立面，实则只选了一方 |
| Contradiction avoidance 矛盾回避 | Treating contradictions as "factors to balance" 把矛盾当作"需要平衡的因素" |
| Template application 模板套用 | Applying one analysis to all situations, ignoring particularity 用一套分析套所有情况，忽视特殊性 |
| Principal-secondary confusion 主次混淆 | Spending energy on secondary contradictions 在次要矛盾上消耗精力 |
| Nature misjudgment 性质误判 | Using negotiation on irreconcilable contradictions 对不可调和的矛盾搞调和 |
| Static analysis 静态分析 | Treating contradictions as fixed instead of transforming 把矛盾当作固定不变的 |

---

## Theoretical foundation | 理论基础

**Primary source — Mao Zedong's dialectical works:**

- 《矛盾论》(On Contradiction, 1937): Principal vs secondary contradictions, universality and particularity of contradiction, contradiction as the engine of all development, concrete analysis of concrete conditions
- 《关于正确处理人民内部矛盾的问题》(On the Correct Handling of Contradictions Among the People, 1957): Distinguishing antagonistic from non-antagonistic contradictions — the nature of contradiction determines the method of resolution
- 《论十大关系》(On the Ten Major Relationships, 1956): Managing multiple contradictions simultaneously, "walking on two legs," the art of handling a contradiction network rather than a single contradiction

**Western complements:**

- Hegel: thesis-antithesis-synthesis as the logic of development; contradiction as the root of all movement
- Socratic method: systematic questioning to expose contradictions in beliefs (tool for generating antithesis)
- Steel-manning: build the strongest version of the opposing view before attempting synthesis

**Applied frameworks:**

- TRIZ: "every invention problem is a resolvable contradiction" — engineering operationalization
- Kahneman framing effects + Lakoff: contradictions may be frame-dependent, not fact-dependent
- I Ching yin-yang: some oppositions are permanent co-generation, not contradiction-driven synthesis
- Deng Xiaoping's "One Country Two Systems": engineering frameworks where contradictions productively coexist

The cognitive protocol strips all theory and translates these ideas into executable instructions for any reasoning agent.

认知协议剥离了所有理论，将这些思想转译为任何推理 agent 可执行的指令。

---

## Installation | 安装

### Claude Code
```bash
cp cognitive-protocol.md ~/.claude/dialectical-thinking.md
echo '@~/.claude/dialectical-thinking.md' >> ~/.claude/CLAUDE.md
```

### Codex
```bash
cat cognitive-protocol.md >> AGENTS.md
```

### Gemini
Paste `cognitive-protocol.md` into `system_instruction`.

将 `cognitive-protocol.md` 内容粘贴到 `system_instruction` 中。

### Cursor
```bash
cat cognitive-protocol.md >> .cursorrules
```

### Any agent | 任何 agent
Inject `cognitive-protocol.md` (~30 lines) into the system prompt. See [`install/generic.md`](install/generic.md) for details.

将 `cognitive-protocol.md`（约 30 行）注入系统提示词。详见 [`install/generic.md`](install/generic.md)。

---

## File structure | 文件结构

```
dialectical-thinking/
├── README.md                  ← You are here / 你在这里
├── cognitive-protocol.md      ← Core rules (~30 lines, always-on) / 核心规则（约 30 行，始终激活）
├── SKILL.md                   ← Full framework reference / 完整框架参考
├── anti-patterns.md           ← Detailed anti-pattern guide / 反模式详解
├── examples.md                ← Before/after scenarios / 前后对比示例
├── install/
│   ├── claude-code.md         ← Claude Code installation / Claude Code 安装指南
│   ├── codex.md               ← Codex installation / Codex 安装指南
│   ├── gemini.md              ← Gemini installation / Gemini 安装指南
│   └── generic.md             ← Universal guide / 通用安装指南
└── LICENSE                    ← MIT
```

---

## Composability | 可组合性

Dialectical Thinking is a **cognitive base** — it changes how the agent frames problems, not what it produces. It stacks cleanly with any domain skill (coding, design, writing, analysis) because it operates at a different layer.

矛盾论是一个**认知底座**——它改变 agent 的问题框架方式，而非产出内容。它与任何领域技能无冲突地叠加，因为它运行在不同的层级。

### Relationship to other cognitive bases | 与其他认知底座的关系

| Layer 层级 | What it governs 管辖范围 | Example 示例 |
|---|---|---|
| First Principles 第一性原理 | What you build ON — verifying foundations 在什么之上建构——验证基础 | "Audit assumptions before solving" 先审计假设 |
| Dialectical Thinking 矛盾论 | What you build THROUGH — navigating contradictions 通过什么来建构——驾驭矛盾 | "Locate the principal contradiction" 定位主要矛盾 |
| Systems Thinking 系统思维 | What you build WITHIN — understanding feedback loops 在什么之中建构——理解反馈回路 | "Trace second-order effects" 追踪二阶效应 |

All three load as always-on cognitive protocols. No conflicts. Combined: reason from verified foundations (FP), through contradiction dynamics (DT), within systemic feedback (ST).

三者同时加载，始终激活，互不冲突。组合效果：从经过验证的基础出发（第一性原理），通过矛盾的动态（矛盾论），在系统反馈中推进（系统思维）。

---

## License

MIT
