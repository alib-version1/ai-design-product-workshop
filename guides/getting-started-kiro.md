# Getting Started with AWS Kiro

AWS Kiro is an AI-powered IDE that turns plain English descriptions into working code. You do not need any coding experience.

## Vibe mode vs spec mode

Kiro has two modes. Use **vibe mode** today.

| | Vibe mode | Spec mode |
|--|-----------|-----------|
| **What it does** | Generates code directly from your description | Writes requirements docs and architecture plans before touching code |
| **Speed** | Fast — you get a working page in seconds | Slow — significant upfront planning before anything is built |
| **Best for** | Rapid prototyping and experimentation | Production software development |
| **Use today?** | Yes | No |

Spec mode is powerful for real software projects. For a one-day workshop where you want to see and click something quickly, it is the wrong tool. Stick to vibe mode throughout.

**How to make sure you are in vibe mode:** When you open the chat panel, look for the mode selector and choose **Vibe**. If you are ever prompted to generate specs or create task plans, decline and go back to the chat.

## How to use it

1. Open Kiro
2. Create a new file: go to File > New File, name it `something.html`
3. Open the AI chat panel — click the chat icon in the left sidebar
4. Describe what you want in plain English
5. Review the generated code and click Accept, or copy it into your file
6. Save the file
7. Double-click the file to open it in your browser

## Tips

- Describe what you want visually: "a page with a heading and a green button that says Continue" — not technical language
- Work on one page at a time
- Preview your work by double-clicking the .html file — it opens in your browser
- If the output is not right, follow up in the same chat: "make the heading bigger" or "add a back link"

## When things go wrong

| Problem | What to try |
|---------|------------|
| Nothing happening | Check your file is saved with a `.html` extension |
| Output looks wrong | Describe what you want differently — be more specific about layout and colours |
| Links between pages do not work | Tell Kiro "the back link should go to start.html" |
| Styling looks off | Say "make this look like GOV.UK with dark text and a green button" |
| Code looks broken | Paste the whole file into the chat and say "fix this" |

## Try it now

1. Create a file called `test.html`
2. Open the Kiro chat panel
3. Type: "Create a simple HTML page with a heading that says Hello and a short paragraph. Clean and professional. All CSS embedded."
4. Accept or copy the output into your file
5. Save it
6. Double-click to open in your browser

You should see a web page. That is all there is to it.
