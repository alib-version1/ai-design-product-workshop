# Service Mapping Prompts

Use these prompts with **M365 Copilot** during Sprint 1 to map your service and identify where to intervene. Copy the prompt, replace the `[bracketed sections]` with your own content, and paste into Copilot.

---

## Prompt 1: Service Blueprint Generator

```
Service: [brief description]
Journey: [paste or describe steps]

Create a blueprint with layers:
1. FRONT STAGE - User actions
2. FRONT STAGE - Touchpoints (website, letter, phone, face-to-face)
3. FRONT STAGE - Visible staff actions
4. BACK STAGE - Internal actions
5. SUPPORT PROCESSES - Systems, databases, policies, third parties

Table format with columns per journey stage.
```

---

## Prompt 2: Pain Points and Opportunities

```
Based on this service blueprint: [paste]

Identify:
1. Top 3-5 pain points from the user's perspective
2. How digital tools could help at each point
3. Which has the highest value if solved
4. Which is most feasible to prototype today

We need to pick one focus area.
```

---

## Prompt 3: As-Is vs To-Be Comparison

```
Current service: [paste or describe how it works today]

We are proposing: [describe the new/improved version]

Compare:
- What stays the same (and why that is fine)
- What changes for users
- What changes for staff or operations
- What is removed entirely
- What risks are introduced by the change
- What quick wins could be delivered without a full rebuild

Keep it practical. We are looking for what to prioritise.
```

---

## Prompt 4: Failure Modes and Edge Cases

```
Service journey: [paste or describe]
Intended user: [persona summary]

Think through what goes wrong:
1. What happens if the user makes a mistake part-way through?
2. What if the user needs to stop and come back later?
3. What if the information provided is wrong or incomplete?
4. What happens for users who do not have the information requested?
5. What if a supporting system (payment, identity, letter) fails?

For each failure: what does the user experience, and what should happen instead?
```

---

## Prompt 5: Metrics and Success Criteria

Use this when preparing your presentation. It helps you articulate impact, not just what you built.

```
Service or feature we are designing: [description]
Problem we are solving: [summary]

Define what success looks like if this were built and deployed:
1. User outcome metrics (what gets better for users? e.g. fewer calls to the helpline, faster completion)
2. Operational metrics (what gets better for the team delivering this? e.g. reduced manual processing)
3. Business or policy metrics (what gets better for the organisation? e.g. higher completion rates, lower cost per transaction)
4. How would we know within 3 months if this prototype had solved the problem?

Keep metrics specific. "Users are happier" is not a metric. "50% reduction in calls about application status" is.
These are indicative and aspirational — the point is to show we have thought about impact, not to commit to numbers.
```

---

## Prompt 6: Business Rules and Decision Logic

Use this to surface the rules that govern how a service works — the decision points, conditions, and data dependencies that determine what happens and to whom. These rules directly shape what your prototype needs to show: which questions to ask, in what order, and what happens based on the answers.

```
Service: [brief description]
The part of the service we are focusing on: [describe the journey or process]

Help us identify the business rules and decision logic:

1. What are the key decision points in this journey? (moments where the service does something different based on conditions)
2. For each decision point:
   - What rule governs it? (e.g. "if the applicant is under 18, a parent must co-sign")
   - What data or information is needed to make the decision?
   - Where does that data come from — the user, a system, a staff member, a third party?
   - What happens on each branch? (the "if this, then that")
3. Are there eligibility rules, time limits, or thresholds that gate access to the service?
4. Are any rules set by legislation or policy vs rules that are just "how it has always been done"?

Present as a clear list or decision table. Flag anything where the rule is unclear or the team disagrees — those are the areas that need clarification before building.
```

---

## Prompt 7: Trade-offs and What Happens Next

Use this when preparing your presentation. It sharpens the product thinking by making explicit what you chose not to do, and helps frame the realistic next steps if the idea is worth pursuing.

```
Problem statement: [paste]
What we prototyped: [describe the screens and journey you built]
What we left out: [anything you discussed but deliberately excluded]

Help us articulate:
1. Trade-offs — what did we deliberately not address, and why? What are the risks of leaving these out?
2. What would break first — if this were real, what is the first thing that would fail or frustrate users that our prototype does not cover?
3. Next steps — if this prototype is compelling, what is the realistic next move?
   - Is this a discovery (we need to research whether the problem is real)?
   - Is this an alpha (we need to test whether this approach works)?
   - Is this a business case (we need to make the case for investment)?
   - What evidence would we need to gather?
4. Quick wins — is there anything from this prototype that could be done without a full project? (e.g. content improvements, process changes, small fixes)

Be practical. Frame this as what a product manager would take into a prioritisation or governance conversation.
```
