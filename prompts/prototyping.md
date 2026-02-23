# Prototyping Prompts

Use these prompts with **AWS Kiro** or **GitHub Copilot in VS Code** during Sprint 2 to generate HTML pages for your prototype. Copy the prompt, replace the `[bracketed sections]` with your own content, and paste into the chat.

Prompts 1–7 produce self-contained HTML files with embedded CSS — no internet needed. Save the file, double-click to open in your browser, and iterate.

Prompt 8 uses the real GOV.UK Frontend library loaded via CDN — **this requires an internet connection**. Use it when you want production-accurate components and class names.

> **Which approach should I use?** Prompts 1–7 are faster to get started and work offline. Prompt 8 is more accurate and better for teams with interaction designers who want to use the real GOV.UK component structure.

---

## Prompt 1: Start Page

```
Create a complete HTML page styled like a GOV.UK start page.

Service: [name]
The page tells users they can: [what]
Before starting, users need: [key info]
Button text: Start now

Style like GOV.UK: #0b0c0c text, #1d70b8 links, #0f7a52 start button with white text. Blue header (#1d70b8) with white "GOV.UK" text, light blue-grey footer (#f4f8fb). Max width 960px. Clean and professional.
All CSS embedded. No external files.
```

---

## Prompt 2: Question Page

```
Create a complete HTML page styled like a GOV.UK question page.

The page asks: [question]
Input type: [text input / radios / checkboxes / textarea / date input]
Options (if radios/checkboxes): [list]
Hint text: [if needed]
Next page: [filename]
Back link to: [filename]

h1 is the question. Green Continue button. Proper form labels. Accessible.
Same GOV.UK styling. All CSS embedded.
```

---

## Prompt 3: Check Your Answers Page

```
Create a complete HTML page using the GOV.UK Check your answers pattern.

Summary list showing:
[list each question and an example answer]

Each row has: question, answer, Change link.
Heading: Check your answers before submitting.
Green Submit button.
Same GOV.UK styling. All CSS embedded.
```

---

## Prompt 4: Confirmation Page

```
Create a complete HTML confirmation page styled like GOV.UK.

Service: [name]
Reference number: [example]
What happens next: [steps and timescales]
Contact: [if applicable]

Green confirmation banner with the reference number. Next steps in plain English.
Same GOV.UK styling. All CSS embedded.
```

---

## Prompt 5: Status Page

```
Create a complete HTML status page styled like GOV.UK.

Heading: [what the user is checking]
Current status: [text] displayed as a coloured tag/badge
Key dates: [list]
Timeline of events: [list with dates and descriptions]
Section: "Is anything needed from me?" with answer
Section: "What happens next?" with explanation

Same GOV.UK styling. All CSS embedded.
```

---

## Prompt 6: Connect Your Pages

Once you have built multiple pages, use this prompt to link them together:

```
I have these HTML pages:
[list each filename and what it does]

The journey order is: [describe flow]

Check and fix:
- Back links point to the correct previous page
- Continue/Submit buttons link to the correct next page
- Navigation works end to end
- Styling is consistent
```

---

## Prompt 7: Accessibility Check

Use this to review any page you have built:

```
Review this HTML: [paste]

Check against WCAG 2.2 AA:
- Form labels and legends
- ARIA labels where needed
- Colour contrast
- Keyboard navigation
- Skip to main content link
- Heading hierarchy

Give me specific fixes with code.
```

---

## Prompt 8: Using the Real GOV.UK Frontend Library

Use this when you want pages that use the **actual GOV.UK Design System** rather than hand-coded CSS. This produces more accurate prototypes and teaches the correct component names and patterns.

```
Create a complete HTML page using the official GOV.UK Frontend library (v5).

REQUIRES INTERNET — loads via CDN. Do not use this prompt offline.

Use this exact document structure:

<!DOCTYPE html>
<html lang="en" class="govuk-template govuk-template--rebranded">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>[Page title] — [Service name] — GOV.UK</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/govuk-frontend@5/dist/govuk/govuk-frontend.min.css">
</head>
<body class="govuk-template__body">
  <script>
    document.body.className += ' js-enabled'
  </script>
  <!-- page content here -->
  <script type="module">
    import { initAll } from 'https://cdn.jsdelivr.net/npm/govuk-frontend@5/dist/govuk/govuk-frontend.min.js'
    initAll()
  </script>
</body>
</html>

Page type: [start page / question page / check your answers / confirmation / task list / status]
Service name: [name]
Page content: [describe what goes on this page]

Requirements:
- Use govuk-* CSS classes exactly as documented at design-system.service.gov.uk
- Do NOT write custom CSS to mimic GOV.UK — use the real components
- Use the correct HTML structure for each component (fieldsets, legends, labels)
- Header: govuk-header with service name
- Footer: govuk-footer
- Main content inside <main class="govuk-main-wrapper">
- Wrap everything in <div class="govuk-width-container">

Components to include: [e.g. govuk-button, govuk-input, govuk-radios, govuk-checkboxes, govuk-summary-list, govuk-task-list, govuk-inset-text, govuk-notification-banner]
```

**Why use this prompt?** The earlier prompts use custom inline CSS that looks like GOV.UK but is not the real thing. This prompt uses the GOV.UK Frontend package — the same library used in production government services. The component class names, HTML structure, and JavaScript behaviours are accurate. The `govuk-template--rebranded` class applies the 2025 GOV.UK rebrand styling automatically.

---

## Prompt 9: Task List Page

Use this for multi-part services where users complete sections in stages.

For the most accurate result, use this with **Prompt 8** (real GOV.UK Frontend). The version below uses embedded CSS.

```
Create a complete HTML page styled like the GOV.UK task list pattern.

Service: [name]
Task sections:
- Section 1 heading: [name]
  - Task: [name] — [Not started / In progress / Completed / Cannot start yet]
  - Task: [name] — [status]
- Section 2 heading: [name]
  - Task: [name] — [status]

Show a line at the top: "You have completed X of Y sections."
Each task name is a link (or placeholder link with href="#").
Status tags: "Completed" in green, "In progress" in blue, "Not started" in grey, "Cannot start yet" in grey with no link.
GOV.UK styling. All CSS embedded.
```

---

## Prompt 10: Interruption / Information Page

Use this when users need to read important information before continuing.

```
Create a complete HTML page styled like a GOV.UK interruption or information page.

Service: [name]
Heading: [what the user needs to know]
Body content: [the key information — what to expect, what will happen, how long it takes]
Use GOV.UK inset text for any warnings or important callouts: [text]
Button text: [Continue / I understand / Accept and continue]
Back link to: [filename]

GOV.UK styling. All CSS embedded.
```

---

## Prompt 11: Address Lookup Page

```
Create a complete HTML page styled like a GOV.UK address lookup flow.

Service: [name]
Step: Postcode entry

The page has two states — show both in the same file using a simple JavaScript toggle:

State 1 (default — visible on load):
- A text input labelled "Postcode" with hint text "For example, SW1A 2AA"
- A "Find address" button
- A "Enter the address manually" link below the button that switches to State 2

State 2 (hidden on load — shown when the link is clicked):
- Manual address entry fields:
  - Address line 1
  - Address line 2 (optional)
  - Town or city
  - County (optional)
  - Postcode
- A "Back to postcode lookup" link that switches back to State 1

Use plain JavaScript (no libraries) to toggle between states.
GOV.UK styling, accessible labels, all CSS and JS embedded in the file.
```
