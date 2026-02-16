# Prototyping Prompts

Use these prompts with **GitHub Copilot in VS Code** during Sprint 2 to generate HTML pages for your prototype. Copy the prompt, replace the `[bracketed sections]` with your own content, and paste into Copilot Chat.

Each page will be a self-contained HTML file with embedded CSS. Save it, double-click to open in your browser, and iterate.

---

## Prompt 11: Start Page

```
Create a complete HTML page styled like a GOV.UK start page.

Service: [name]
The page tells users they can: [what]
Before starting, users need: [key info]
Button text: Start now

Style like GOV.UK: #0b0c0c text, #1a65a6 links, #0f7a52 start button with white text. Blue header (#1d70b8) with white "GOV.UK" text, light blue-grey footer (#f4f8fb). Max width 960px. Clean and professional.
All CSS embedded. No external files.
```

---

## Prompt 12: Question Page

```
Create a complete HTML page styled like a GOV.UK question page.

The page asks: [question]
Input type: [text input / radios / checkboxes / textarea]
Options (if radios/checkboxes): [list]
Hint text: [if needed]
Next page: [filename]
Back link to: [filename]

h1 is the question. Green Continue button. Proper form labels. Accessible.
Same GOV.UK styling. All CSS embedded.
```

---

## Prompt 13: Check Your Answers Page

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

## Prompt 14: Confirmation Page

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

## Prompt 15: Status Page

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

## Prompt 16: Connect Your Pages

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

## Prompt 17: Accessibility Check

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
