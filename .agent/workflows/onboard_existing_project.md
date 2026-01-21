---
description: Procedures for onboarding the agent into an existing/legacy project.
---
# Onboard Existing Project

## Trigger
Run this when adding the `.agent` folder to a project that already has code (Legacy).

## Steps

### 1. Discovery & Analysis (The Scan)
*   **Action**: Scan the root directory and key subfolders (`src`, `app`, `lib`).
*   **Goal**: Identify the technology stack automatically.
    *   *Look for*: `package.json` (Node), `requirements.txt` (Python), `docker-compose.yml`, `csharp`, `java`, etc.

### 2. Memory Initialization
*   **Action**: Update `.agent/AI_MEMORY.md`.
    *   Set **Status** to "Active Development".
    *   Fill **Technology Stack** with findings from Step 1.
    *   List **Key Constraints** (e.g., "Uses generic css", "Has Testing Library").

### 3. Knowledge Base Population
*   **Action**: Create `knowledge/project_structure.md`.
    *   Document the detected folder structure.
*   **Action**: Check for existing guidelines.
    *   If `.eslintrc` exists -> Create `knowledge/lint_rules.md`.
    *   If `README.md` exists -> Extract architectural rules to `rules.md`.

### 4. Skill Generation (Bootstrap)
*   **Action**: Use `skill-creator` to generate skills relevant to the found stack.
    *   *Example*: If React found -> Create `skill-react-component`.
    *   *Example*: If SQL found -> Create `skill-database-query`.

## Command Shortcut
// turbo-all
