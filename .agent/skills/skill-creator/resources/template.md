---
name: {{skill_name}}
description: {{short_description}}
---

# {{Skill Title}}

## Context
{{Description of what this skill does and the persona the agent should adopt.}}

## When to use
- {{Trigger 1}}
- {{Trigger 2}}

## Workflow
You must follow this process strictly to ensure quality and strict adherence to project standards.

### 1. Analysis & Preparation
- **Review Context**: Read relevant files to understand the current state.
- **Compatibility Check**: Ensure your planned actions are compatible with the existing codebase and previous changes.
- **Stack Identification**: Identify the project's technology stack (do not assume).

### 2. Planning
- Outline the steps you will take.
- Identify potential risks or side effects.

### 3. Execution
- Implement the changes or perform the action.
- Use `task_boundary` to track progress if the task is complex.

### 4. Verification (CRITICAL)
- **Test**: Run available tests or perform manual verification of your changes.
- **Validate**: Ensure the change meets the user's original request.
- **Fix**: If verification fails, analyze why, fix the issue, and verify again.

### 5. Detailed Documentation
- Record a detailed summary of what was done.
- Note any specific decisions made during execution.
- **Memory Update**: Update `.agent/AI_MEMORY.md` if this task changed key project information.
