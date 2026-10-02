# STAR Method Builder

Guided builder for STAR interview answers (Situation, Task, Action, Result). Four guided sections with prompts and word targets, a live assembled preview, a bank of common behavioral questions, and locally saved answers. No external services, a structured writing aid that runs entirely in your browser.

**Live demo:** https://0xelitesystem.github.io/star-method-builder/

## Use

1. Pick a behavioral question from the list.
2. Fill in Situation, Task, Action, and Result, watching each word count against its target.
3. Check the assembled preview and the total word count.
4. Click Copy full answer, or give it an Answer name and click Save to keep it in this browser.

## Why this exists

A STAR answer falls apart when the setup runs long and the result has no number. This tool gives each part a word target and shows the assembled answer as you type. It is one HTML file with no AI, no account, and no tracking, released under the MIT license.

## Features

- Four labeled sections, each with a one-line explanation, memory-jogging prompt questions, and a live word count with per-section guidance (Situation and Task: 30 to 60 words; Action: 60 to 120; Result: 30 to 60, with a number if possible)
- Live assembled full-answer preview that joins the parts into flowing paragraphs
- Total word count against a 150 to 300 word target (roughly 60 to 90 seconds spoken)
- Bank of 15 common behavioral questions (conflict, failure, leadership, deadline, ambiguity, feedback, and more) to frame the exercise
- Save, load, and delete multiple named answers in localStorage
- Copy button for the full answer, including the framing question
- Tips section: quantify results, say "I" not "we" for your actions, keep the situation short
- Light and dark theme, keyboard friendly, works offline

## How it works

Type into the four sections and the tool counts words, colors the counters against the guidance ranges, and assembles the preview live. Situation and Task merge into one setup paragraph, Action and Result stand alone, matching how a spoken answer actually flows. Saving writes a named snapshot (question plus all four parts) to localStorage; loading restores it exactly.

There is no generation, no scoring engine, and no network use. It is a structured writing aid: the structure, the prompts, and the word targets do the coaching, and every word is yours.

## Privacy

All client-side. Nothing leaves the browser: no requests, no analytics, no accounts. Saved answers live in your browser's localStorage on your device only; clearing site data removes them.

Saved answers are kept under the localStorage key `star-method-builder.answers.v1`. Nothing else is stored.

## Run locally

```
git clone https://github.com/0xelitesystem/star-method-builder
cd star-method-builder
```

Open `index.html` in a browser, or serve the folder with `python -m http.server` and visit http://localhost:8000.

## Build

No build step. The whole tool is one `index.html` file.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT. Copyright 0xelitesystem 2026.
