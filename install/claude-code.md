# Install — Claude Code

## Quick install

```bash
# 1. Copy cognitive protocol to Claude's config
cp cognitive-protocol.md ~/.claude/dialectical-thinking.md

# 2. Add reference in CLAUDE.md
echo '@~/.claude/dialectical-thinking.md' >> ~/.claude/CLAUDE.md
```

## What gets loaded where

| File | Destination | Purpose |
|---|---|---|
| `cognitive-protocol.md` | `~/.claude/dialectical-thinking.md` | Always-on core rules (~30 lines) |
| `SKILL.md` | `~/.claude/skills/dialectical-thinking/SKILL.md` | Full reference (loaded on demand) |
| `anti-patterns.md` | `~/.claude/skills/dialectical-thinking/anti-patterns.md` | Detailed anti-pattern guide |
| `examples.md` | `~/.claude/skills/dialectical-thinking/examples.md` | Before/after reference |

## Full install (with skill files)

```bash
# 1. Core rules
cp cognitive-protocol.md ~/.claude/dialectical-thinking.md

# 2. Skill files
mkdir -p ~/.claude/skills/dialectical-thinking
cp SKILL.md ~/.claude/skills/dialectical-thinking/
cp anti-patterns.md ~/.claude/skills/dialectical-thinking/
cp examples.md ~/.claude/skills/dialectical-thinking/

# 3. Register in CLAUDE.md
echo '@~/.claude/dialectical-thinking.md' >> ~/.claude/CLAUDE.md
```

## Verify

Ask Claude Code: "What are the dialectical thinking cognitive rules you're following?" It should list the six sections from `cognitive-protocol.md`: map the contradiction network, locate the principal contradiction, judge the nature, monitor transformation, steel-man the opposition, concrete analysis of concrete conditions.

## Stacking with other cognitive bases

If `~/.claude/first-principles.md` or `~/.claude/systems-thinking.md` are already referenced in `CLAUDE.md`, no changes needed. All protocols load independently. First Principles governs what you reason FROM; Dialectical Thinking governs what you reason THROUGH; Systems Thinking governs what you reason WITHIN. No conflicts.

## Uninstall

```bash
rm ~/.claude/dialectical-thinking.md
rm -rf ~/.claude/skills/dialectical-thinking
# Remove the @~/.claude/dialectical-thinking.md line from ~/.claude/CLAUDE.md
```
