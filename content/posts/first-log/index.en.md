---
title: "The Day I Got Hugo Running Locally"
date: 2026-01-16
draft: true
tags:
  - log
  - setup
summary: "[SOLVED] A log of setting up Hugo on macOS while confirming it worked on localhost."
---

Today, I finally set up a place to keep my records.
I built this blog locally using Hugo.

To be honest, I felt a little uneasy before starting.
But when I saw the title appear on the screen,
I thought, “Yes, this is my place.”

---

## What I did today
- Installed Hugo using Homebrew
- Created a new site with `hugo new site`
- Set up the PaperMod theme
- Started the local server with `hugo server -D`
- Checked the page displayed at localhost:1313

## Commands I ran
```bash
# Install Hugo
brew install hugo

# Check Hugo version
hugo version

# Create a new site
hugo new site hachiware-log

# Start the local server (including drafts)
hugo server -D
```

![localhostで表示できた画面](hugo-localhost.png)

*↑The first screen I saw when the site loaded locally.*

## Where I stumbled
- I hesitated about where to edit hugo.toml

  → I decided to edit it in VSCode.

- I wasn’t sure if it was okay to run commands from VSCode

  → Since running commands from the VSCode terminal is fine, I just double-checked the working directory and proceeded.

## What I achieved
- I got Hugo running locally on my Mac
- I realized, “This can be an article.”

---

## A note to my future self

This place is not for finishing things.
It’s for leaving records of the steps I take.

Don’t rush — just keep goin