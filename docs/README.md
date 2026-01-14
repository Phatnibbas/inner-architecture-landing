# Agent Skills & Framework Setup

## Overview
This workspace installs a structured `.claude/skills` layout with protocols, methodologies, templates, and safety framework docs. It is modeled after the referenced repositories and the directory structure you described.

## Sources
- https://github.com/ruvnet/claude-flow
- https://github.com/alirezarezvani/claude-skills
- https://github.com/levnikolaevich/claude-code-skills (reference; README not found at the default URL)

## Structure
- `.claude/skills/mcp-agents`: protocols and orchestration patterns
- `.claude/skills/safe-framework`: quality gates, benchmarking, batch runner
- `.claude/skills/agent-templates`: 12 agent templates
- `.claude/skills/skill-packages`: manifest and package layout
- `.claude/skills/hierarchy`: 3-level hierarchy and lazy loading

## Key Capabilities
- Hive Mind pattern and SPARC methodology
- Consensus protocols and neural pattern learning
- GitHub PR/Issue automation templates
- Multi-pass quality gates
- Performance benchmarking and batch runner
- Terms dictionary

## Verification
Check `.claude/skills/STATUS.md` for Level 90 status and installation notes.

## Batch Runner
- Runner: `.claude/skills/safe-framework/batch_runner.py`
- Sample plan: `.claude/skills/safe-framework/batch-plan.sample.yaml`

## Auto-Link for Antigravity
Run this once per project to link global rules:

```powershell
powershell -ExecutionPolicy Bypass -File "$env:USERPROFILE\.claude\skills\safe-framework\link-antigravity-rules.ps1"
```

Or double-click:
- `C:\\Users\\ninhh\\.claude\\skills\\safe-framework\\link-antigravity-rules.cmd`

## New Project Helper
Creates a project folder and links the global rules:

```powershell
powershell -ExecutionPolicy Bypass -File "$env:USERPROFILE\\.claude\\skills\\safe-framework\\new-project.ps1"
```

Or double-click:
- `C:\\Users\\ninhh\\.claude\\skills\\safe-framework\\new-project.cmd`

## Auto-Run Options
Watcher (default base: `$env:USERPROFILE\source`):

```powershell
powershell -ExecutionPolicy Bypass -File "$env:USERPROFILE\\.claude\\skills\\safe-framework\\watch-projects.ps1"
```

Install watcher on startup:
- `C:\\Users\\ninhh\\.claude\\skills\\safe-framework\\install-watch-startup.cmd`

Git hooks (run per repo after `git init`):
- `C:\\Users\\ninhh\\.claude\\skills\\safe-framework\\install-git-hooks.cmd`

Workspace auto-run task:
- The link script creates `.vscode/tasks.json` with `runOn: folderOpen`.

## Next Steps
- Extend templates with domain-specific skills
- Integrate with your preferred agent runtime
