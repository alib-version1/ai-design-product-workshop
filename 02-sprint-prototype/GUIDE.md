# Sprint 2: Build Your Prototype

## Before you start: load your guardrails

Before your first prompt, tell your AI tool to follow the project guardrails. In your AI tool chat, type:

> "Please follow the rules in @GUARDRAILS.md for this project."

This sets the AI to work the way your team needs — plain English output, no technical setup required, GOV.UK styling applied by default. You only need to do this once per session.

## Your brief

Turn your problem, persona, and service map into something you can show — and take away. A working prototype that someone can click through, that demonstrates the concept, and that tells the story of how this service could work for your user.

This is not production code. It does not need to be pixel-perfect. It needs to be good enough to demo and clear enough that someone can understand the idea by clicking through it.

## How to spend your time

**First 15 minutes — agree what to build.** Which part of the journey, what flow, what content, and what the prototype needs to show by the end. Before diving into pages, check your prototype scope against your service blueprint from Sprint 1. Ask: are we prototyping the right moment in the service? Does the front-stage we are building make sense given the back-stage process we mapped? If your blueprint showed a step where the user switches channel (e.g. goes from online to phone) or where a back-stage process determines what the user sees next, make sure your prototype accounts for that — even if it is just a page that says "at this point, a caseworker reviews your application." Think about GOV.UK patterns.

**Next 90 minutes — build.** One person drives your AI coding tool (Kiro or GitHub Copilot). Everyone else directs — content, layout, flow, user perspective. Use the prompts in [prompts/prototyping.md](../prompts/prototyping.md). Work one page at a time: generate it, check it in the browser, move on.

**Last 30 minutes — refine.** Look at what you have built as a team. Does the journey make sense? Is the content clear? Fix the things that matter for your presentation.

## How each role contributes

- **Interaction Designers**: Layout, components, flow between pages — does this follow GOV.UK patterns?
- **Content Designers**: Every word on every page — headings, labels, hint text, error messages. Plain English.
- **User Researchers**: Would our persona understand this? Where would they get stuck?
- **Service Designers**: Does the front-stage make sense given the back-stage? Keep checking the prototype against the service blueprint — are we showing the right part of the journey?
- **Product Managers**: What is in scope? Keep the team focused on the parts of the prototype that tell the story.
- **Business Analysts**: Process logic. What questions need asking? What are the rules?
- **Delivery Managers**: Time. Keep the team moving. Make sure something is ready to present.
- **Directors and Deputy Directors**: What makes this compelling? What questions will the audience ask?

## Tips

- **If using Kiro, stay in vibe mode.** If Kiro starts generating spec documents or task plans, switch back to Vibe mode in the chat panel. You want code, not planning docs.
- One page at a time. Get it rendering in the browser before starting the next one.
- Journey over pixels. A clear flow with rough styling beats a beautiful page that goes nowhere.
- If you get stuck, paste your code into the chat and describe what is wrong.
- Look at the [example pages](../examples/) for GOV.UK-styled HTML you can reference.
- Use the [content and language prompts](../prompts/content-and-language.md) to get the words right.

## When you are ready to present

Use the [presentation template](../templates/presentation.md) to structure your 5–7 minute slot.

## Are you ready to present?

Before presentations, check:

- [ ] You can click through your journey from start to finish without breaking
- [ ] Your persona's name or situation appears in the prototype
- [ ] Every step has a clear heading
- [ ] Your problem statement is on your first slide
- [ ] You know which part of the prototype best shows the value of your idea
- [ ] You could hand this prototype to a colleague and they would understand what it is for

---

**Previous:** [Sprint 1 — Define Your Problem](../01-sprint-define/GUIDE.md)
