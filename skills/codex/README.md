# Codex Skill

Enable Claude Code to invoke the Codex CLI (`codex exec` and session resumes) for automated code analysis, refactoring, and editing workflows.

## Prerequisites

- `codex` CLI installed and available on `PATH`
- Codex configured with valid credentials
- Verify with `codex --version`

## Usage

Invoke the skill in Claude Code:

```
/codex
```

Or ask Claude directly:

```
Use codex to analyze this repository and suggest improvements.
```

## When to Use

- Large-scale refactoring across many files
- Deep code analysis requiring extended reasoning
- Getting a second opinion on architectural decisions
- Complex debugging sessions

## Thinking Tokens

By default, this skill suppresses thinking tokens (stderr output) using `2>/dev/null` to avoid bloating Claude Code's context window. If you want to see the thinking tokens for debugging, explicitly ask Claude to show them.
