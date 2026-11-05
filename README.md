# teach-me

A Claude skill that turns Claude into a tutor for anything you want to learn: a school or uni subject, an exam, a professional skill, a language, a hobby. It plans across sessions toward your goal, tracks what you know against the full scope of the topic (a syllabus dot point by dot point, if you have one), and keeps notes on how you learn. It also runs small experiments on its own teaching, so it gets better at teaching you over time.

## Get it

**Latest version:** [teach-me.zip](https://github.com/HazzardRust/teach-me/releases/latest/download/teach-me.zip). This link always points to the newest release.

- **Claude app (web, desktop or mobile):** upload `teach-me.zip` as a skill in Claude's settings.
- **Claude Code:** copy the `teach-me/` folder into `~/.claude/skills/`, or clone this repo and symlink it so `git pull` updates it.

To update, download the zip again and replace the old skill. Your notes and logs live in your own Claude docs, so replacing the skill doesn't touch them.

## Needs

- The **Claude Docs** connector. The tutor keeps its notes, tracker, learning log and a whiteboard in Claude docs.
- Optional: voice mode for the teaching part, and a phone for sending photos of your working.

## Use it

1. Start a chat and say **"study time"**. The first time, it walks you through setup (topic, goal or exam date, syllabus or scope, devices) and creates its docs.
2. A setup that works well: the chat open on a computer with the Whiteboard beside it, and photos of handwritten working sent into the same chat from your phone.
3. Teaching can happen in text or voice, your choice. The tutor suggests voice for conceptual work (ideas, explaining) and text for skill work like equations and full questions, with photos of your working. Voice mode doesn't load skills by itself, so always *start* in text chat.
4. End by switching back to text chat and saying **"done"**, so the session gets recorded.

## What's inside

```
teach-me/
  SKILL.md                  the teaching method
  references/first-run.md   setup and doc templates for a new user
  references/examples.md    worked examples of the key moves
```

## Changes

Improvements come from real study sessions. Each release notes what changed.
