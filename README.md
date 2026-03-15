# Socratic

A portable Claude Code skill for structured thinking. Two modes, one principle: **open at the right moment, close at the right moment.**

## Modes

- **LEARN** — deepen understanding through Socratic questioning (5 levels)
- **PRODUCE** — turn clear thinking into concrete output (5 steps)

## Install

```bash
git clone https://github.com/kadenn/socratic.git
cd socratic
./setup
```

This creates a symlink in `~/.claude/skills/socratic` — no dependencies needed.

## Usage

In any Claude Code conversation:

```
/socratic learn <topic>
/socratic produce <topic>
```

## How it works

**LEARN mode** asks questions instead of giving answers. It progresses through 5 levels of depth: surface definition → distinction → mechanism → edge cases → application. You advance only when you demonstrate genuine understanding, not keyword matching.

**PRODUCE mode** closes loops instead of reopening them. It progresses through 5 steps: define output → lock thesis → draft structure → refine → finalize. Each step locks a decision — no going back.

**Drift detection** — if you start building when you should be learning (or questioning when you should be shipping), the skill names it and asks if you want to switch modes consciously.

## Uninstall

```bash
rm ~/.claude/skills/socratic
```
