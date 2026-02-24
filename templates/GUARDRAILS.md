# GUARDRAILS.md — Project Guardrails for AI Prototyping

**To use this file:** When starting a new conversation with your AI tool, type:
> "Please follow the rules in @GUARDRAILS.md for this project."

You do not need to understand or modify this file — just load it at the start of each session.

---

## Purpose

This file sets the rules for how your AI tool should behave during this prototyping project. It keeps things simple, consistent, and appropriate for a non-technical team.

---

## Core Principles

| Principle | What it means |
|-----------|---------------|
| **Prototype Focus** | Build things that look and work like real services — not perfect code |
| **Plain English** | Always communicate with the user in plain English. Avoid technical jargon. If you must use a technical term, explain it simply in brackets. |
| **Sensible Defaults** | Make reasonable choices without asking the user to decide technical details |
| **One thing at a time** | Build one page or one component at a time — not the whole service in one go |
| **Show, don't explain** | Produce working output rather than describing what you are going to do |

---

## Technical Standards

- All pages must be self-contained HTML files — no external frameworks, no package installations, no command-line steps
- CSS must be embedded directly in the HTML file
- JavaScript, if needed, must also be embedded in the HTML file
- Pages must open by double-clicking the file in a file explorer — no local server required
- Do not ask the user to run terminal commands, install packages, or set up a development environment

---

## When Requirements Are Ambiguous

Use these defaults without asking the user:

| If the user does not specify… | Default to… |
|-------------------------------|-------------|
| Colour scheme | GOV.UK colours — dark navy text, blue links, green primary button |
| Font | System default sans-serif (no custom font imports) |
| Page width | Maximum 960px, centred |
| Layout | Single column, clean and readable |
| Button style | Large, filled, high contrast |
| Form fields | Standard label above input, with visible border |
| Navigation | Simple back link at the top, no complex menus |
| Header | Simple bar with service name |
| Footer | Simple bar with minimal content |

---

## Notes for AI Implementation

- Match the visual style of GOV.UK (gov.uk) where possible — the design is clean, accessible, and familiar to UK public sector users
- Prioritise clarity and usability over visual complexity
- Always communicate in plain English — no jargon, no technical instructions directed at the user
- If a prompt is ambiguous, make a reasonable assumption and build it — explain what you assumed at the end, not before
- Do not ask the user to copy-paste code between files or run scripts
- When generating multiple pages, create each one as a separate file
- Use descriptive, readable file names (for example: `check-your-answers.html`, not `page3.html`)

---

## The section below sets technical defaults — it is for the AI tool, not for you to understand or change.

## Tech Stack

- HTML5, vanilla CSS, vanilla JavaScript only
- No frameworks (no React, Vue, Bootstrap, Tailwind, etc.)
- No build tools, no npm, no package managers
- No CDN links unless specifically requested
- Single-file output per page

---

## When Things Go Wrong

If the output does not look right:

1. **Describe what is wrong in plain English** — "the button is in the wrong place" or "the heading is too small"
2. **Ask for one change at a time** — this makes it easier for the AI to get it right
3. **If it keeps going wrong**, describe the current state of the page and say: "Here is what I have so far — [describe the problem] — please fix it"

You do not need to understand the code. You just need to describe what you see versus what you want.
