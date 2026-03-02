---
version: 0.1.0
description: Protocol to use Research, Plan and Implement method in agent coding projects
type: context
---
## artifact structure

Keep these files as your single source of truth during the project:

1. **ADRs (`docs/adr/*.md`):** Architecture decisions and rules (The "Why").
2. **Design Docs (`docs/dd/00X-*.md`):** Your roadmap for each feature (The "How").
3. **Features (`docs/feature_list.yaml`):** Current backlog state.
4. **Session (`.claude/MEMORY.md`):** Volatile notes from current session.

## RPI workflow (Research → Plan → Implement)

This workflow is mandatory for any change affecting >1 file or touching critical logic. Apply in strict sequence.

### Phase R: Research

**Discovery**
- Map all files the change will touch.
- Search for cross-dependencies (imports, exports, references).
- Identify relevant data schemas (types, interfaces, models).

**Analysis**
- Extract current logic (what it does, boundaries, edge cases).
- Document expected vs. actual behavior.
- Flag technical constraints or patterns already established in the project.

**Trigger to advance to Plan:** When you have clarity on the complete scope.

### Phase P: Planning

**Design Doc numbered** in `docs/dd/` (eg: `docs/dd/001-design_auth.md`)

Structure:
```
# Design: [Brief name]

## Findings (from Phase R)
- [What you found, current behavior, limitations]

## Objective
- [What changes and why]

## Proposed changes
- [ ] Item 1: brief description
- [ ] Item 2: brief description
- [ ] Item N: brief description

## Testing
- Unit: [what they cover]
- Integration: [key flows to validate]
- Edge cases: [3-5 critical cases]

## Risks
- [Possible breakages, if any]
```

**Architecture Decision Record** (if needed)

If the plan involves architectural changes (new patterns, major refactors, tech choices), create an ADR in `docs/adr/` before implementation.

ADR structure (`docs/adr/001-jwt_refresh_strategy.md`):
```
# ADR-001: JWT Refresh Strategy

## Status
Accepted (or: Proposed, Rejected, Superseded)

## Context
Brief explanation of the issue that motivated this decision.

## Decision
What was decided and why.

## Consequences
What follows from this decision (positive and negative impacts).
```

**Validation before implementing:**
- [ ] Design Doc approved by user or key stakeholders.
- [ ] Each change checkbox is atomic (can be done in 1 commit).
- [ ] If architecture changes exist, ADR is written and approved.

**Trigger to advance to Implement:** Explicit user approval.

### Phase I: Implementation

**Execution**
- One Design Doc checkbox = one atomic commit.
- Commit pattern: `feat(scope): description` or `fix(scope): description`.
- Each commit must pass tests before marked "done".

**Testing inline**
- Run local tests after each step.
- If they fail, diagnose and adjust the current step (don't advance).
- Document in Design Doc what differed from the plan.

**Finalization**
- All checkboxes ✓.
- All tests pass (unit + integration).
- Update `docs/feature_list.yaml` when moving to `completed`.
- Add one line to changelog if it exists.

### tracking features (docs/feature_list.yaml)

Keep a lean record of what's in progress. Structure:
```yaml
auth_redesign:
  status: in_progress
  phase: implement
  design_doc: docs/dd/001-design_auth.md
  adr: docs/adr/001-jwt_refresh_strategy.md
  
  checkpoints:
    - id: 1
      task: "Refactor JWT middleware"
      status: completed
    - id: 2
      task: "Add refresh token logic"
      status: in_progress
  
  blockers: []
  last_updated: "2025-03-02"

notifications_system:
  status: not_started
  phase: research
  design_doc: null
  adr: null
  
  checkpoints: []
  blockers: []
  last_updated: "2025-03-01"
```

**How to use it:**
- `status`: not_started, in_progress, completed, blocked.
- `phase`: research, plan, implement (aligned with RPI).
- `design_doc`: Reference to design file in `docs/dd/` (null if doesn't exist yet).
- `adr`: Reference to architecture decision in `docs/adr/` (null if no architecture changes).
- `checkpoints`: Each Design Doc checkbox is a checkpoint here.
- `blockers`: Issues blocking progress (empty if none).
- `last_updated`: Date to know if it's fresh.

### context management (when chat grows)

**Compaction signals:**
- Chat >50 messages.
- You start repeating instructions or context.
- Response speed degrades.

**Protocol:**
1. Pause implementation.
2. Update `.claude/MEMORY.md` with:
   - What was completed (checkpoints ✓).
   - What's pending (open checkpoints).
   - Current active Design Doc and its status.
   - Any important decisions made.
3. Propose: "Context full. Updated MEMORY.md. Suggest restarting session to continue with clarity."
4. On next session:
   - Read `MEMORY.md` first.
   - Load active Design Doc.
   - Continue from where we left off.

