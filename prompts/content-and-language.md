# Content and Language Prompts

Use these prompts with **M365 Copilot** to get the words right — headings, labels, hint text, error messages, and plain English content. Useful in both Sprint 1 (when framing the problem) and Sprint 2 (when building pages).

---

## Prompt 1: Content Review

```
Service: [description]
Current experience: [what content/comms users currently receive]

Review the content design:
- Where might language confuse users?
- What information do users need at each stage?
- How could it be simplified?
- Which GOV.UK content patterns apply?

Plain English. GOV.UK style guide.
```

---

## Prompt 2: Error and Help Content

```
Service where users need to: [task]

Generate:
1. Validation error messages (clear, specific, actionable)
2. Help text for complex questions
3. Confirmation messaging
4. What to say when things go wrong or users need to wait

GOV.UK patterns. Specific not generic.
```

---

## Prompt 3: Page Content in GOV.UK Style

Use this to draft the actual content for a page in your prototype — not just review existing content, but write it from scratch following GOV.UK content design patterns.

```
This is a [start page / question page / information page / confirmation page] for a service that: [describe what the service does]

The user has reached this point because: [what they have done so far in the journey]
What they need to do on this page: [the task or decision]
What they need to know: [key information]

Write the full page content:
- Page title (as it would appear in the browser tab): [Service name] — GOV.UK
- H1 heading (clear, task-focused — tells the user what to do, not what the page is about)
- Body content in plain English — short sentences, active voice, front-loaded
- Any hint text for form fields (help users understand what is being asked, without repeating the question)
- Button text (specific — "Send your application" not "Submit")
- Inset text or warning text if the user needs to know something important before continuing

Follow the GOV.UK style guide: no jargon, no Latin, no "please", no "you should". Address the user as "you". One idea per sentence. Reading age 9.
```

---

## Prompt 4: Form Questions and Hint Text

The hardest content design task in government services is writing questions that users actually understand. Use this to draft question pages — the wording, hint text, and options that determine whether someone can complete the service.

```
Service: [brief description]
We need to ask the user about: [what information we need and why]

For each question we need to ask:
1. Write the question as an H1 heading — phrased as something the user can answer, not a data field label (e.g. "What is your date of birth?" not "Date of birth entry")
2. Write hint text that helps without repeating the question (e.g. "For example, 31 3 1980" not "Enter your date of birth in the format DD MM YYYY")
3. If the answer is a choice (radios/checkboxes), write the options in language users would use — not policy language or system codes
4. Explain why we are asking (for the team's benefit, not for the page) — if you cannot explain why, the question might not be needed
5. Flag any questions where the wording depends on policy or legal definitions that should be checked

One question per page unless they are closely related. Follow the GOV.UK "one thing per page" pattern.
```

---

## Prompt 5: Simplify Policy Language

Use this when your service includes content that comes from legislation, policy documents, or operational guidance that was not written for a public audience.

```
This is the original text from [a policy document / legislation / internal guidance / a letter template]:

[paste the source text]

This text is shown to users when they are: [describe the context — what the user is doing and what they need to understand]

Rewrite this for a GOV.UK service page:
- Plain English, reading age 9
- Active voice — "We will send you" not "A notification will be issued"
- Short sentences — ideally under 25 words
- Front-loaded — the most important information first
- No jargon, acronyms, or Latin (use "for example" not "e.g.", "and" not "&")
- Address the user as "you" and the organisation as "we"
- Remove anything the user does not need to know at this point in the journey

Show the before and after so the team can see what changed and why. Flag any changes where the simplification might alter the legal or policy meaning — those need checking.
```
