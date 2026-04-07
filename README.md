# grill-me

A Claude Code skill for structured interrogation of plans, designs, and ideas. It acts as a sharp, collegial interviewer that stress-tests your thinking by probing assumptions, surfacing risks, and tracking decisions.

## Installation

1. Copy the `grill-me` directory into your Claude Code skills folder:

    ```
    ~/.claude/skills/grill-me/
    ```

    The directory structure should be:

    ```
    ~/.claude/skills/grill-me/
    ├── SKILL.md
    ├── README.md
    └── evals/
        └── evals.json
    ```

2. Claude Code will automatically detect the skill. No additional configuration is required.

## Compatibility

This skill works with:

- Claude Code CLI (terminal)
- Claude Code desktop app (the Code tab in Claude Desktop on Mac/Windows)

It does **not** work with the regular Claude desktop app or claude.ai — skills are a Claude Code-specific feature.

## Usage

Invoke the skill by saying any of:

- "grill me"
- "grill me about [topic]"
- "stress test my plan"
- "poke holes in this"

The skill will ask for a short session name, then walk through your plan branch by branch — challenging assumptions, finding gaps, and recording decisions in a persistent session file at `grill-me-sessions/<plan-name>.grill.md`.

## What it does

- Interviews you about your plan without executing it
- Tracks decisions, deferred items, and open threads in a session file
- Reads relevant code and docs to ask informed questions
- Resumes previous sessions where you left off

## What it does not do

- Write code, scripts, or deliverables
- Execute the plan being discussed
- Review or refactor existing code (use code review tools for that)
