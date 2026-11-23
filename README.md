# Claim Verification — by The Ask Why Company

Verify important factual claims with traceable sources, dates, provenance, corroboration, and explicit uncertainty.

Read the skill: [skills/claim-verification/SKILL.md](skills/claim-verification/SKILL.md)

Works with Claude (Claude Code, Claude.ai) and any tool that reads the open [Agent Skills](https://agentskills.io) `SKILL.md` format.

## Install in Claude

**Claude Code:**
```
/plugin marketplace add theaskwhy/claim-verification
/plugin install claim-verification@claim-verification
```

Or from the full catalogue: `/plugin marketplace add theaskwhy/skills` then `/plugin install claim-verification@theaskwhy`.

**Manual:** copy `skills/claim-verification/` into `~/.claude/skills/` (personal) or `.claude/skills/` (project).

**Claude.ai:** zip the `skills/claim-verification` folder and upload it under Settings → Capabilities → Skills.

## Use with other AI agents

This skill uses the open **Agent Skills** standard. The same `SKILL.md` works with compatible tools including OpenAI Codex, Cursor, Gemini CLI, GitHub Copilot, Windsurf, Antigravity, OpenCode, and Goose.

**Quick install:** the open-source `skills` installer detects supported tools:
```
npx skills add theaskwhy/claim-verification
```

**Manual:** copy `skills/claim-verification/` into your tool's skills folder:

| Tool | Personal (all projects) | One project |
|---|---|---|
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |
| OpenAI Codex | `~/.codex/skills/` | `.agents/skills/` |
| Cursor | `~/.cursor/skills/` | `.cursor/skills/` |
| Gemini CLI / Antigravity | `~/.gemini/skills/` | `.gemini/skills/` |
| GitHub Copilot | `~/.copilot/skills/` | `.github/skills/` |
| Windsurf | — | `.windsurf/skills/` |
| Any spec-compliant agent | — | `.agents/skills/` |

For tools without skills support, paste `SKILL.md` into the tool's rules or instructions file.

## Licence

MIT. See [LICENSE](LICENSE).
