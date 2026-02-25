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
1. Minimum viable journey (3–5 steps in the user's journey, end to end)
2. What to include vs leave out
3. The single most important thing the prototype must demonstrate
```

---

## Prompt 4: Persona Generator

> **Important:** This generates a proto-persona — a hypothesis based on your team's assumptions and professional experience. It is not a validated research output. Treat it as a starting point to be tested with real users, not as evidence.

```
Service: [brief description]
Main users: [description]
Key problem: [description]

Create a realistic proto-persona (a hypothesis based on our team's assumptions, not validated research):
- Name, age, situation
- Goals
- Frustrations with the current experience
- Context (when/how they interact)
- A quote capturing how they feel
- Digital confidence level

A real person, not a segment. Grounded in practical reality.
Label the output clearly as "Proto-persona — to be validated through user research."
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

---

## Prompt 10: Four Discovery Questions

Use this prompt before anything else if your team is unsure whether the problem is real or well-defined enough to prototype. It runs a quick discovery review in 5 minutes.

```
Service: [brief description]
What we think is going wrong: [describe the problem]

Answer these four questions as if you are a discovery researcher doing a rapid evidence review. Be direct. If evidence is thin, say so.

1. Is there actually a problem? Who struggles, how often, and what is the consequence for them when it goes wrong?
2. Who experiences it differently? Are there groups — by age, channel, digital confidence, circumstance — who are more affected than others?
3. What does policy or legislation actually require? What is genuinely mandated versus what is just how things have always been done?
4. How do people currently get through it? What workarounds, shortcuts, or alternative channels do people use to cope?

End with: what is the strongest evidence for this problem, and what are we assuming without evidence?
```

Use the output to sharpen your problem statement before moving on. If the AI's answer feels generic or unconvincing, your problem needs more definition before you prototype it.

---

## Prompt 11: Research Synthesis — What We Already Know

Use this when your team has professional experience of the problem but no formal research to hand. It helps structure what you collectively know into organised evidence and — crucially — surfaces where the gaps are.

```
We are a team working on: [service description]
The problem we are focusing on: [problem statement]

Between us, we have professional experience of this service. Here is what we know from our work — observations, things users have told us, patterns we have seen, complaints we have heard:

[paste bullet points, notes, or free-text from the team — the messier the better]

Help us organise this into:
1. Themes — group related observations together and name each theme
2. Strength of evidence — for each theme, is this based on direct observation, second-hand reports, or assumption?
3. Who is affected — which user groups does each theme apply to?
4. Gaps — what important questions are NOT answered by what we know? What would a user researcher want to investigate next?

Be honest about where evidence is thin. Label assumptions clearly.
```

---

## Prompt 12: User Stories and Acceptance Criteria

Use this to translate your workshop outputs into structured requirements. Useful for business analysts who want a tangible takeaway, and for anyone who needs to explain what the prototype represents in delivery terms.

```
Problem statement: [paste]
Persona: [paste]
Prototype scope: [describe the user journey your prototype covers — what the user does at each step and what each step shows]

Generate user stories and acceptance criteria for the journey we are prototyping:

For each screen or step, write:
- A user story in the format: "As a [persona name], I need to [action], so that [outcome]"
- 2-4 acceptance criteria in the format: "Given [context], when [action], then [result]"
- Any business rules or conditions that apply (e.g. "if the user selects X, they are routed to Y")

Keep language plain. These are draft stories to be refined — not a final backlog.
```
