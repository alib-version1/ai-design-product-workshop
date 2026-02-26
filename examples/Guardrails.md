# Project Guardrails

> This file sets technical boundaries for prototype development. It's designed for non-technical users — you don't need to understand or modify it. Just load it and the AI will follow these rules automatically.

---

## Core Principles

1. **Simplicity First**: Choose the simplest solution that meets the requirements. Avoid over-engineering.

2. **User Experience Priority**: All user interfaces must follow the GOV.UK Design System and MoJ Design System patterns and components, implemented using the GOV.UK Frontend and MoJ Frontend toolkits.

3. **Reliability Over Features**: A smaller set of working features is better than more features that break.

4. **Sensible Defaults**: When a decision isn't specified, choose the most common/expected behaviour.

5. **Prototype Focus**: This is rapid prototyping, not production development. Prioritise getting something working that can be demonstrated and tested with users.

---

## Technical Standards

### Tech Stack
- **Frontend**: GOV.UK Frontend and MoJ Frontend toolkits (mandatory)
- **Templating**: Nunjucks
- **Backend**: Node.js with Express
- **Database**: SQLite for any data persistence
- **Rendering**: Server-side rendering only

### User Interface
- Use GOV.UK Design System and MoJ Design System patterns and components for all views
- Follow the "one thing per page" principle
- Implement using GOV.UK Frontend and MoJ Frontend toolkits
- Use GOV.UK notification banners for success/error messages
- Confirmation for destructive actions (delete, cancel, etc.)

### Code Quality
- All code must include basic error handling
- User-facing errors should be friendly and actionable ("Something went wrong. Please try again.")

---

## When Requirements Are Ambiguous

If the specification doesn't address something, use these defaults:

| Situation | Default Behaviour |
|-----------|------------------|
| How to handle deleted items? | Soft delete (hide, don't destroy) |
| Pagination needed? | Yes, if lists could exceed 20 items |
| Search needed? | Yes, if lists could exceed 10 items |
| Date/time format | Readable format (e.g., "5 January 2025") |
| Currency format | GBP (£) unless specified |

---

## Constraints

- **Do not** implement payment processing
- **Do not** store sensitive data
- **Do not** build features that weren't specified — ask for clarification instead
- **Do** flag any potential security or privacy concerns

---

## Prototype Constraints

This is rapid prototyping for testing ideas with users, not production development.

- The prototype runs in isolation on a laptop — it cannot connect to real external systems
- Where the real service would connect to external systems (case management, payment services, etc.), simulate realistic responses with sample data
- Include realistic sample data so demonstrations feel real
- Focus on getting something working that can be demonstrated, not production-ready code
- Create a simple run script (e.g., `start.sh` or `start.bat`) that starts the prototype with a single command
- When the prototype is running, tell the user how to view it in their browser

---

## When Things Go Wrong

If the user reports something isn't working:

1. Ask them to describe what they see versus what they expected
2. Ask if they can share a screenshot
3. Review the plan (@plan.md), requirements (@requirements.md) and problem statement (@problem-statement.md) to check if the implementation matches the intent
4. Fix the issue and explain what was wrong in simple terms

---

## Notes for AI Implementation

When in planning mode:
- Reference these guardrails for all technical decisions
- Do not ask the user for technology preferences — use the defaults above
- If requirements conflict with these guardrails, flag it but follow the requirements
- Remember the user is not technical — avoid jargon and explain decisions simply

When in agent mode:
- Write clean, readable code with comments for non-obvious logic
- Create a simple README explaining how to run the project
- Include sample data so the user can see the application working immediately
- Focus on getting a working prototype, not production-ready code