# Step 5: Build Your First Page

**Tool:** AWS Kiro or GitHub Copilot in VS Code

You are going to generate a single web page using your AI coding tool. This is your first time — the only goal is to see it work.

## Open your AI chat panel

**If you are using AWS Kiro:**
1. Open Kiro
2. Click the chat icon in the sidebar to open the AI chat panel
3. Make sure it is set to **Vibe** mode — not Spec. Vibe mode generates code directly from your description. Spec mode creates planning documents first, which you do not need today. If Kiro asks you to review a spec or task plan, you are in the wrong mode.

**If you are using GitHub Copilot in VS Code:**
1. Open VS Code
2. Press **Ctrl+Shift+I** (Windows/Linux) or **Cmd+Shift+I** (Mac) to open the Copilot Chat panel

## What to do

1. Open your AI tool (as above)
2. Create a new file and save it as `start.html`
3. Copy the prompt below and paste it into the chat
4. Accept or copy the code it generates into your file
5. Save the file
6. Double-click the file in your file explorer to open it in a browser

## Prompt to copy

```
Create a complete HTML page styled like a GOV.UK start page.

Service name: Check the progress of your application
The page tells users they can: see where their application is, check if anything is needed from them, and find out when to expect a decision
Before starting, users need: their application reference number
Button text: Start now

Style it like GOV.UK:
- Background: white
- Text colour: #0b0c0c
- Link colour: #1d70b8
- Start button: #0f7a52 with white text, large
- A simple header bar (blue background #1d70b8, white "GOV.UK" text)
- A simple footer (light grey background, #f4f8fb)
- Maximum width 960px, centred
- Clean, readable, professional

All CSS must be embedded in the HTML file. No external files or links.
The page must be complete and ready to open in a browser.
```

## What just happened

You described a page in plain English. Your AI tool turned it into a working web page. Open it in your browser — you should see something that looks like a government start page.

It will not be perfect. The styling might be slightly off. The layout might need tweaking. That is fine. The point is: **you went from a description to a working page in under a minute.**

In Sprint 2, you will build multiple connected pages for your own problem. This was the first step.

---

**Previous:** [Step 4 — Decide What to Prototype](STEP-4-SCOPE.md) | **Done — return to the** [Challenge overview](README.md)
