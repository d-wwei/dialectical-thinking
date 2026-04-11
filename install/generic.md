# Install — Generic (Any Agent)

## Principle

Dialectical Thinking is a cognitive protocol — a set of always-on reasoning rules. It works with any LLM agent by injecting `cognitive-protocol.md` (~30 lines) into the system prompt.

矛盾论是一个认知协议——一组始终激活的推理规则。通过将 `cognitive-protocol.md`（约 30 行）注入系统提示词，适用于任何 LLM agent。

## Installation pattern

### Step 1: Core rules (required)

Inject the contents of `cognitive-protocol.md` into your agent's system prompt. This is the only required file. It contains six rules:

1. Map the contradiction network
2. Locate the principal contradiction
3. Judge the nature of each contradiction
4. Monitor contradiction transformation
5. Steel-man the opposing side
6. Concrete analysis of concrete conditions

### Step 2: Reference material (optional)

Make `SKILL.md`, `anti-patterns.md`, and `examples.md` available as retrievable context. The agent can reference these when deeper analysis is needed.

Options:
- RAG: Index the files and let the agent retrieve relevant sections
- Context injection: Include `SKILL.md` in the system prompt for always-available full reference
- On-demand: Provide files when the user requests detailed dialectical analysis

### Step 3: Verify

Ask your agent: "What dialectical thinking rules are you following?"

Expected response should reference: contradiction network mapping, principal contradiction identification, nature judgment (reconcilable vs irreconcilable), transformation monitoring, steel-manning, concrete analysis of concrete conditions.

## Token budget

| File | Approximate tokens | When to load |
|---|---|---|
| `cognitive-protocol.md` | ~500 | Always (system prompt) |
| `SKILL.md` | ~3,000 | On demand or always |
| `anti-patterns.md` | ~3,500 | On demand |
| `examples.md` | ~4,000 | On demand |

Minimum viable install: `cognitive-protocol.md` only (~500 tokens).

## Framework-specific patterns

### LangChain / LangGraph
```python
from langchain_core.messages import SystemMessage

with open("cognitive-protocol.md") as f:
    protocol = f.read()

messages = [SystemMessage(content=protocol), ...]
```

### OpenAI API
```python
with open("cognitive-protocol.md") as f:
    protocol = f.read()

response = client.chat.completions.create(
    model="gpt-4o",
    messages=[
        {"role": "system", "content": protocol},
        {"role": "user", "content": "Your prompt here"}
    ]
)
```

### Anthropic API
```python
with open("cognitive-protocol.md") as f:
    protocol = f.read()

response = client.messages.create(
    model="claude-sonnet-4-20250514",
    system=protocol,
    messages=[{"role": "user", "content": "Your prompt here"}]
)
```

### Custom agent frameworks
Prepend `cognitive-protocol.md` contents to whatever system prompt mechanism your framework uses. The protocol is framework-agnostic — it's just text instructions.

## Stacking with other cognitive bases

Dialectical Thinking stacks cleanly with other cognitive protocols:
- **First Principles**: Verifies foundations → Dialectical Thinking maps contradictions among verified foundations
- **Systems Thinking**: Maps feedback loops → Dialectical Thinking identifies which loops contain contradictions
- **Tacit Knowledge**: Governs output quality → Dialectical Thinking governs problem framing

Load order doesn't matter. No conflicts between protocols.
