# Install — Claude Code

> **Recommended**: Run `./install.sh` from the repo root for automated installation with dual-mode support (@ reference + inline fallback).
> The manual steps below are for reference or troubleshooting.

## Quick install

```bash
# 1. Inject core rules into CLAUDE.md (direct content injection — works on all versions)
cat cognitive-protocol.md >> ~/.claude/CLAUDE.md
```

## What gets loaded where

| File | Destination | Purpose |
|---|---|---|
| `cognitive-protocol.md` | `~/.claude/CLAUDE.md` (appended) | Always-on core rules (~30 lines) |
| `SKILL.md` | `~/.claude/skills/dialectical-thinking/SKILL.md` | Full reference (loaded on demand) |
| `anti-patterns.md` | `~/.claude/skills/dialectical-thinking/anti-patterns.md` | Detailed anti-pattern guide |
| `examples.md` | `~/.claude/skills/dialectical-thinking/examples.md` | Before/after reference |

## Full install (with skill files)

```bash
# 1. Core rules (inject directly into CLAUDE.md)
cat cognitive-protocol.md >> ~/.claude/CLAUDE.md

# 2. Skill files
mkdir -p ~/.claude/skills/dialectical-thinking
cp SKILL.md ~/.claude/skills/dialectical-thinking/
cp anti-patterns.md ~/.claude/skills/dialectical-thinking/
cp examples.md ~/.claude/skills/dialectical-thinking/

# 3. (Core rules already injected in step 1)
```

## Verify

Ask Claude Code: "What are the dialectical thinking cognitive rules you're following?" It should list the six sections from `cognitive-protocol.md`: map the contradiction network, locate the principal contradiction, judge the nature, monitor transformation, steel-man the opposition, concrete analysis of concrete conditions.

## Stacking with other cognitive bases

If First Principles or Systems Thinking is already injected into `CLAUDE.md`, no changes needed. All protocols load independently. First Principles governs what you reason FROM; Dialectical Thinking governs what you reason THROUGH; Systems Thinking governs what you reason WITHIN. No conflicts.

## Uninstall

```bash
# Remove the Dialectical Thinking section from ~/.claude/CLAUDE.md (search for "# Dialectical Thinking — Cognitive Protocol" header)
rm -rf ~/.claude/skills/dialectical-thinking
```
