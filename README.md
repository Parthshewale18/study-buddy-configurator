# Study Buddy Configurator

A single-page tool that generates a personalised Claude system prompt for AI-assisted studying — built during Anthropic's AI Fluency course.

Instead of a generic "help me study" prompt, this configurator walks you through your learning profile, style, and boundaries, then outputs a ready-to-use system prompt designed to make Claude act as a **guide**, not an answer machine.

## Why

Pasting your homework into an AI and getting the answer back doesn't teach you anything. This tool encodes good tutoring practice — asking questions before explaining, checking understanding before moving on, never doing the work for you — into a prompt tailored to how *you* learn.

## How it works

The configurator is a 5-step wizard:

1. **Profile** — your name, subject, learning goal, and current knowledge level
2. **Learning Style** — how you like to encounter new concepts, what helps when you're stuck, preferred tone, and how much guidance you want before getting a straight answer
3. **Protocols** — pick the study modes you want available: Problem-Solving, Concept Review, Exam Prep, Writing Support, Reading Comprehension, General Planning, Assignment Planning, and Reflection
4. **Boundaries** — rules to keep the AI in "tutor" mode (e.g. never answer assessment questions directly, check understanding before new concepts) plus anything to avoid
5. **Generate** — a complete system prompt is assembled from your answers, with a live preview updating as you type

## Using the generated prompt

1. Fill out the form and click **Generate My Study Buddy**
2. Copy the prompt from the output box (or the live preview sidebar)
3. Paste it into **Claude.ai → Settings → Custom Instructions** for persistent use, or as the first message in a new chat
4. Start a session with something like *"I want to do a problem-solving session on thermodynamics"*
5. Switch modes anytime mid-conversation by naming a different protocol

## Tech

Plain HTML, CSS, and vanilla JavaScript — no build step, no dependencies, no backend. All state lives in the browser; nothing is saved or sent anywhere.

## Running locally

```bash
git clone https://github.com/Parthshewale18/study-buddy-configurator.git
cd study-buddy-configurator
open index.html
```

Or just open `index.html` directly in any browser.

## Credits

Built as part of Anthropic's AI Fluency course.
