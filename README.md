# Claude Code Skills

Common Claude Code skills for the SFD-Hackathon team.

## Quick Install (All Skills)

```bash
git clone https://github.com/SFD-Hackathon/claude-skills.git /tmp/claude-skills && \
cp -r /tmp/claude-skills/skills/* ~/.claude/skills/ && \
rm -rf /tmp/claude-skills
```

## Available Skills

| Skill | Description | Prerequisites |
|-------|-------------|---------------|
| [codex](skills/codex/) | Invoke OpenAI Codex CLI for code analysis and refactoring | `codex` CLI installed |

## Install Individual Skills

### Codex

```bash
git clone https://github.com/SFD-Hackathon/claude-skills.git /tmp/claude-skills && \
mkdir -p ~/.claude/skills/codex && \
cp -r /tmp/claude-skills/skills/codex/* ~/.claude/skills/codex/ && \
rm -rf /tmp/claude-skills
```

## Usage

Once installed, invoke skills in Claude Code using:

```
/<skill-name>
```

For example:
```
/codex
```

Or ask Claude directly:
```
Use codex to analyze this repository.
```

## Adding New Skills

1. Create a new directory under `skills/<skill-name>/`
2. Add required files:
   - `SKILL.md` - Skill instructions (required)
   - `README.md` - Documentation (recommended)
3. Update the "Available Skills" table in this README
4. Submit a PR

### Skill File Format

`SKILL.md` should follow this format:

```markdown
---
name: skill-name
description: Brief description of when to use this skill
---

# Skill Name Guide

## Instructions for Claude Code
...
```

## Directory Structure

```
claude-skills/
├── README.md
└── skills/
    ├── codex/
    │   ├── SKILL.md
    │   └── README.md
    └── <new-skill>/
        ├── SKILL.md
        └── README.md
```

## License

MIT
