# Install — Codex

## Quick install

```bash
cat cognitive-protocol.md >> AGENTS.md
```

## Full install

```bash
# 1. Core rules (append to AGENTS.md)
cat cognitive-protocol.md >> AGENTS.md

# 2. Reference files (place in project for context)
mkdir -p .cognitive/dialectical-thinking
cp SKILL.md .cognitive/dialectical-thinking/
cp anti-patterns.md .cognitive/dialectical-thinking/
cp examples.md .cognitive/dialectical-thinking/
```

## Verify

Ask Codex: "What dialectical thinking rules are active?" It should reference: contradiction network mapping, principal contradiction location, nature judgment, transformation monitoring, steel-manning, concrete analysis.

## Notes

- `cognitive-protocol.md` is ~30 lines — minimal token overhead.
- Codex loads `AGENTS.md` automatically per session.
- Reference files in `.cognitive/` are available when Codex needs deeper guidance.
