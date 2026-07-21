<h1 align="center">This repository has moved</h1>

<h2 align="center"><a href="https://github.com/kadenn/skills">Continue at kadenn/skills</a></h2>

<p align="center">
  <a href="https://github.com/kadenn/skills"><img alt="Continue to kadenn/skills" src="https://img.shields.io/badge/CONTINUE%20TO-kadenn%2Fskills-2ea44f?style=for-the-badge&amp;logo=github"></a>
</p>

<p align="center"><strong>This repository is a read-only legacy snapshot.</strong></p>
<p align="center">Use the monorepo for future updates, issues, and contributions.</p>
<p align="center"><code>gh skill install kadenn/skills socratic</code></p>

---

# Socratic

A portable Claude Code skill for structured thinking. One principle: **open at the right moment, close at the right moment.**

## Skills

- **`/socratic`** — adaptive mode, reads your intent and steers accordingly
- **`/learn`** — deepen understanding through Socratic questioning
- **`/produce`** — turn clear thinking into concrete output

## Install

```bash
git clone https://github.com/kadenn/socratic.git
cd socratic
./setup
```

This creates symlinks for all three skills in `~/.claude/skills/` — no dependencies needed.

## Usage

```
/socratic <topic>     — let the skill read your intent and guide you
/learn <topic>        — explicit questioning mode
/produce <topic>      — explicit production mode
```

## How it works

**`/learn`** asks questions instead of giving answers. It moves through layers of depth — definition, distinction, mechanism, edge cases, application — going as deep as needed. You advance when you demonstrate genuine understanding, not keyword matching.

**`/produce`** closes loops instead of reopening them. It guides you through defining output, locking direction, drafting structure, refining, and finalizing. Each step locks a decision — no going back without a conscious choice.

**`/socratic`** reads the situation. If you're exploring, it asks questions. If you're ready to ship, it helps you converge. Drift gets named, not enforced.

**Drift detection** — if you start building when you should be learning (or questioning when you should be shipping), the skill names it and lets you decide.

## Uninstall

```bash
rm ~/.claude/skills/socratic ~/.claude/skills/learn ~/.claude/skills/produce
```
