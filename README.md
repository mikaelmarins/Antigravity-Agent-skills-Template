# Antigravity Agent Template 🧠

This repository contains a robust, "State of the Art" cognitive framework for **Google Antigravity** agents. It transforms a standard workspace into an intelligent, context-aware environment with long-term memory, rigorous engineering processes, and self-replicating capabilities.

## 🚀 Key Features

*   **Long-Term Memory**: Persistent context via `AI_MEMORY.md` ensures the agent never forgets the project goal or stack.
*   **Meta-Skills**: Includes `skill-creator` to generate new agent capabilities that follow strict engineering standards.
*   **Strategic Planning**: Includes `skill-brainstorm` to turn vague ideas into detailed implementation plans.
*   **Governance**: `rules.md` and `knowledge/` folder to enforce security and coding standards automatically.

## 📂 Structure

```text
.
├── .agent/
│   ├── AI_MEMORY.md       # 🧠 The Brain: Current state, stack, and decisions.
│   ├── rules.md           # ⚖️ The Law: Immutable security & quality rules.
│   ├── scratchpad.md      # 📝 Temporary notes for the agent.
│   ├── skills/            # 🛠️ Active Tools
│   │   ├── skill-creator/ # Meta-skill that creates other skills.
│   │   └── skill-brainstorm/ # PM skill for planning & requirements.
│   ├── workflows/         # ⚙️ Standard Operating Procedures (SOPs).
│   └── knowledge/         # 📚 Static Reference Docs (Style Guides, Specs).
└── README.md              # This file.
```

## 🛠️ Included Skills

### 1. Skill Creator (`skill-creator`)
*   **Role**: Senior Prompt Engineer.
*   **Function**: Generates new skills for the agent.
*   **Behavior**: It refuses to create "lazy" skills. It forces a template that includes Analysis, Planning, Execution, Verification, and Documentation steps.

### 2. Brainstorm & Planning (`skill-brainstorm`)
*   **Role**: Product Manager & Solutions Architect.
*   **Function**: Interviews the user to gather requirements (Stack, Docker, Mobile-first, etc.) and generates a concrete Action Plan.

## 🏁 How to Use

1.  **Clone this template** into your new project folder.
2.  **Initialize**:
    *   Open `AI_MEMORY.md` and check the status.
    *   (Optional) Edit `.agent/rules.md` if you have specific team rules.
3.  **Start Planning**:
    *   Ask the agent: *"Use the brainstorm skill to plan a new [App Name] project."*
    *   The agent will interview you and update `AI_MEMORY.md` with the defined stack.
4.  **Create Skills**:
    *   Ask: *"Create a skill to handle [Specific Task, e.g., Database Migrations]."*
    *   The agent uses `skill-creator` to generate a rigorous, verified skill for that task.

## 🧠 Philosophy

This template operates on the principle of **Context-Aware Agents**. By maintaining a live `AI_MEMORY.md` and strict `rules.md`, we ensure that:
1.  **Context is King**: The agent always knows *what* it is building and *how*.
2.  **Safety First**: Security rules are injected into every session.
3.  **Evolution**: The agent improves its own tools via `skill-creator`.

## 🔄 Using in Existing Projects (Legacy)

To add this brain to a project that **already exists**:

1.  Copy the `.agent/` folder to your project root.
2.  **Run the Onboarding Workflow**:
    *   Ask the agent: *"Execute the onboard_existing_project workflow."*
3.  **What happens**:
    *   The agent scans your files (`package.json`, etc.).
    *   It auto-fills `AI_MEMORY.md` with your current stack.
    *   It extracts rules from your existing `README.md`.
    *   It proposes new skills based on your code (ex: `skill-react`, `skill-python`).
