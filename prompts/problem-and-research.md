# Problem Framing and User Research Prompts

Use these prompts with **M365 Copilot** during Sprint 1 to define your problem, create personas, and understand your users. Copy the prompt, replace the `[bracketed sections]` with your own content, and paste into Copilot.

---

## Prompt 1: Problem Statement Generator

```
We are a team of [roles] working on improving a government/public service.
The service: [brief description]
The problem: [description]
Users affected: [who]

Help us write a structured problem statement:
- What is the current situation?
- Who is affected and how?
- What is the impact (users, organisation, outcomes)?
- What does good look like?

Plain language. No jargon.
```

---

## Prompt 2: How Might We Generator

```
Based on this problem statement:
[paste]

Generate 5-8 "How Might We" questions as design opportunities.
Each should be:
- Broad enough for creative solutions
- Specific enough to be actionable
- Focused on user outcomes not technology
```

---

## Prompt 3: Scope Definition

```
We have one day to prototype a solution:
[paste problem statement]

Suggest:
1. Minimum viable journey (3-5 screens)
2. What to include vs leave out
3. The single most important thing the prototype must demonstrate
```

---

## Prompt 4: Persona Generator

```
Service: [brief description]
Main users: [description]
Key problem: [description]

Create a realistic persona:
- Name, age, situation
- Goals
- Frustrations with the current experience
- Context (when/how they interact)
- A quote capturing how they feel
- Digital confidence level

A real person, not a segment. Grounded in practical reality.
```

---

## Prompt 5: User Journey Mapper

```
For this persona: [paste]

Map their current journey through: [service description]

Per step:
- What the user does
- What they are thinking and feeling
- What works
- What is frustrating
- Touchpoints (digital, phone, letter, face-to-face)
```

---

## Prompt 6: Assumptions Mapper

```
Problem statement and persona: [paste both]

Identify key assumptions we are making. Per assumption:
- Why it matters (what changes if we are wrong)
- How we could test it
- Confidence (high/medium/low)
```

---

## Prompt 7: Stakeholder Map

```
Service: [brief description]
Problem we are solving: [summary]

Map the stakeholders:
1. Who are the users (direct recipients of the service)?
2. Who are the operators (staff who run or deliver the service)?
3. Who are the sponsors or owners (accountable for the service)?
4. Who are the influencers (policy, legal, compliance, other teams)?
5. Whose buy-in do we need to make this change?

For each group: name, their goal, their concern, their level of influence.
```

---

## Prompt 8: Policy and Constraint Check

```
Service we are designing for: [describe what the service does and who uses it]
What we are proposing to change or prototype: [describe the new feature or improvement]

Help us identify:
1. Policy or legislative constraints that might affect this design
2. Data protection or privacy considerations (GDPR/UK GDPR)
3. Accessibility requirements (WCAG 2.2 AA, Public Sector Bodies Accessibility Regulations)
4. Departmental standards or GOV.UK Service Standard points that apply
5. Questions we should be asking before building anything

Flag anything that would need a legal, policy, or security review before going live.
Note: this is for awareness, not a comprehensive audit. We are a workshop team, not legal counsel.
```

---

## Prompt 9: Decision Log

Use this at the **end of Sprint 1** to capture what your team decided and why, before you start building. It prevents the team from relitigating the same decisions during Sprint 2.

```
We are prototyping: [one sentence description]

Decisions we made in Sprint 1:
[list each decision — e.g. "We chose to focus on the status-checking step, not the application form"]

For each decision, document:
- What we decided
- Why (the rationale)
- What we considered and ruled out
- What would make us revisit this

Format as a simple table with those four columns.
```
