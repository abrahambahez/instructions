---
version: 0.1.0
description: Code rules to work with AI Agents mantaining consistency
type: context
---
## Code Style and Standards

- DO NOT CODE WITHOUT A PLAN: Only execute code after using plan mode or reading a documented plan. If you don't get the plan, ask the user for one
- MVP MINDSET: What's the minimal change that will get the maximum outcome?
- LEAN CODE APPROACH: Less code is always better. For existing code, prefer reducing code over adding code.
- NO COMMENTS: Code must be self-documenting. Use descriptive function names instead of comments. No inline comments except for formal documentation: ex. Python DocStrings, GoDoc, JSDoc for complex functions
- VALIDATE LEAN CHANGES: Every time I ask you for a big change make me know if it can break my main principle of lean code so I can decide if its worth it
- CONSTANT COMMIT CHANGES: Remember me to commit when we finish every feature, functional change, refactoring or every 5 file editions. We use standard conventional commits with one sentence body and small footer.
- USE LANGUAGE BEST PRACTICES: ex. pythonic style + Zen of Python, Effective Go, etc.
- Scope: Don't add features, refactor code, or make "improvements" beyond what was asked. A bug fix doesn't need surrounding code cleaned up. A simple feature doesn't need extra configurability.
- Defensive coding: Don't add error handling, fallbacks, or validation for scenarios that can't happen. Trust internal code and framework guarantees. Only validate at system boundaries (user input, external APIs).
- ABSTRACTIONS: Don't create helpers, utilities, or abstractions for one-time operations. Don't design for hypothetical future requirements. The right amount of complexity is the minimum needed for the current task.

## Documentation rules

- Use the "keep a changelog" standard to write changelogs with semantic versioning

