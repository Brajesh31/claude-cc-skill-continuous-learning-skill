# claude-cc-skill-continuous-learning-skill

A Claude Code skill entry point for a continuous-learning workflow that captures useful development knowledge and improves future task execution.

## Overview

Continuous learning in a development workflow means turning meaningful discoveries into reusable knowledge. Useful examples include project conventions, recurring debugging fixes, validated implementation patterns, and lessons that prevent repeated mistakes.

The current skill definition is intentionally concise. This README provides a practical overview of the continuous-learning purpose and the included configuration and evaluation helper.

## What to Capture

- Repeated project conventions.
- Verified debugging procedures.
- Reusable implementation patterns.
- Important architectural decisions.
- Tool usage discoveries.
- Test and deployment lessons.
- Known failure modes and their fixes.

Avoid saving temporary logs, unverified guesses, secrets, or information that is unlikely to help future work.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-cc-skill-continuous-learning-skill.git ~/.claude/skills/cc-skill-continuous-learning
```

## Usage

Invoke the skill when a task produces a reusable lesson:

```text
/cc-skill-continuous-learning
```

Review `SKILL.md` for the exact operating instructions and `config.json` for the included configuration.

## Learning Workflow

1. Complete the current task.
2. Identify a lesson that is likely to recur.
3. Verify the lesson against actual results.
4. Remove temporary or sensitive details.
5. Store the lesson in a suitable category.
6. Check for duplication or conflict with existing guidance.
7. Evaluate whether the captured knowledge improves future work.
8. Update or retire stale guidance when project behavior changes.

## Included Files

- `SKILL.md`: Main skill definition.
- `config.json`: Workflow configuration.
- `evaluate-session.sh`: Session evaluation helper.
- `README.md`: Overview and usage guidance.

## Evaluation Helper

The repository includes a shell script for session evaluation:

```bash
bash evaluate-session.sh
```

Review the script and its expected inputs before running it. Do not assume that a session evaluation automatically produces a verified or durable learning record.

## Quality Checklist

- Captured knowledge is based on evidence.
- The lesson is reusable.
- Sensitive information is excluded.
- Existing guidance is checked for conflicts.
- The record has enough context to be understood later.
- Stale knowledge can be updated.
- Evaluation results are reviewed before retention.

## Practical Principle

Learning should improve future work, not create a growing archive of noise. Store only knowledge that is verified, reusable, and worth retrieving.
