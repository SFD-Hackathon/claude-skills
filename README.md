# Claude Code Skills

Common Claude Code skills for the SFD-Hackathon team.

## Available Skills

### Codex

Enable Claude Code to invoke the Codex CLI (`codex exec` and session resumes) for automated code analysis, refactoring, and editing workflows.

## Installation

Install all skills to your local Claude Code:

```bash
git clone https://github.com/SFD-Hackathon/claude-skills.git /tmp/claude-skills && \
mkdir -p ~/.claude/skills/codex && \
cp /tmp/claude-skills/SKILL.md ~/.claude/skills/codex/ && \
cp /tmp/claude-skills/README.md ~/.claude/skills/codex/ && \
rm -rf /tmp/claude-skills
```

Or install manually:

1. Clone this repository
2. Copy the skill files to `~/.claude/skills/<skill-name>/`
3. Restart Claude Code

## Prerequisites for Codex Skill

- `codex` CLI installed and available on `PATH`
- Codex configured with valid credentials
- Verify with `codex --version`

## Usage

Once installed, invoke the Codex skill in Claude Code:

```
/codex
```

Or simply ask Claude to use Codex:

```
Use codex to analyze this repository and suggest improvements.
```

## Adding New Skills

1. Create a new `SKILL.md` file following the format in existing skills
2. Add documentation to this README
3. Submit a PR

## License

MIT
