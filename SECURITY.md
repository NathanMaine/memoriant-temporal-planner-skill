# Security Policy

## What This Plugin Does

This plugin consists entirely of markdown instruction files (SKILL.md and agent .md files). It contains:
- No executable code
- No shell scripts
- No network calls
- No file system modifications beyond what Claude Code normally does

All operations (reading task files, writing plan output, updating state files) are performed by Claude Code itself using its standard tools, not by any code in this plugin.

## Data Handling

Task plans may contain project-sensitive information (deadlines, dependencies, team assignments). This plugin:
- Never transmits task data externally
- Does not log or persist any information itself — all file operations are performed by Claude Code under user direction
- Does not require any API keys or credentials

## Reporting a Vulnerability

If you discover a security issue, please email nathan@memoriant.com (do not open a public issue).

We will respond within 48 hours and provide a fix timeline.

## Auditing This Plugin

This plugin is easy to audit:
1. All files are markdown — readable in any text editor
2. No `node_modules`, no Python packages, no compiled binaries
3. Review `skills/temporal-planner/SKILL.md` to see exactly what instructions are given to the AI
