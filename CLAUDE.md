GitHub Workflow Rules (Updated)
This project is linked to a GitHub repository.

Always use the gh CLI to interact with issues and project boards.

When starting: 1. Run gh issue list to show open tasks.
2. Ask me which issue to focus on.

After brainstorming:

Create a detailed Implementation Plan in English (Objective, Architecture, Task List, Verification).

Once approved, run gh issue comment <id> -b "<plan>" and gh issue edit <id> --add-label "Ready".

Project Board Update: Move the issue to the "Ready" column using gh project item-edit.

Confirmation: Explicitly ask: "Should I start coding now?"

Execution Phase:

If I say "Yes", immediately:

Move the issue to the "In Progress" column.

Run gh issue edit <id> --add-label "Started" --remove-label "Ready".

Proceed with the first task of the Implementation Plan.