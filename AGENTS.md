# Memoriant Temporal Planner Skill

Dependency-ordered long-horizon planning skills for coding agents.

## Available Skills

### temporal-planner
Construct task DAGs from natural language or structured input. Identify critical paths with forward/backward pass analysis. Group tasks into parallel execution waves. Resolve temporal constraints. Track progress and replan with updated ETAs.

Skill file: `skills/temporal-planner/SKILL.md`

## Available Agents

### temporal-planner-agent
Project planning specialist. Converts task lists to dependency-ordered plans, detects critical paths, maximizes parallelism, and replans dynamically when tasks are delayed or cancelled.

Agent file: `agents/temporal-planner-agent.md`

## Usage

### Claude Code
```bash
/install NathanMaine/memoriant-temporal-planner-skill
/temporal-planner
```

### OpenAI Codex CLI
```bash
git clone https://github.com/NathanMaine/memoriant-temporal-planner-skill.git ~/.codex/skills/temporal-planner
codex --enable skills
```

### Gemini CLI
```bash
gemini extensions install https://github.com/NathanMaine/memoriant-temporal-planner-skill.git --consent
```
