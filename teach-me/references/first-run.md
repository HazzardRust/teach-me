# First-run setup

Read this only when the system hasn't been used yet. Once setup is done, it isn't needed again.

## How to tell it's a first run

Any of these means nothing has been set up:
- section 7 of SKILL.md still has `[link]` placeholders;
- the artifact list (if the Artifact tool can list) has no docs named Teaching Notes, Knowledge Tracker, Psychology Log or Whiteboard;
- the docs exist but their logs are empty (no Session log rows, no subject tabs).

If the docs exist but section 7 is empty (e.g. the skill was reinstalled), don't make new ones: find the old ones, then re-save their links (step 4 below). If only some exist, create just the missing ones.

Never start teaching on a first run until steps 1 to 4 are done. They take a few minutes.

## The setup conversation

This is the learner's first impression, so teach the system the same way the skill teaches a subject: one small question at a time, a sentence or two of explanation when it's needed, never a wall of instructions. Keep it in text chat. Voice mode doesn't load skills.

1. **Welcome, in two or three lines.** Say what this is: a tutor that plans across sessions, keeps notes on what they know and how they learn, and gets better at teaching them over time. Then ask the first question.
2. **Learn their setup, one question per message**, in roughly this order (skip any they've already answered):
   - What do they want to learn, and why: an exam or course (and when is it?), or a skill or interest with no exam (and what would "good enough" look like, with a target date if they have one)? (One subject is enough to start; more can be added any time.)
   - Which exam board or syllabus? (Needed for the syllabus map.) With none, agree the scope map with them instead, built from reputable courses, textbooks or standards.
   - Which devices do they have? Explain what works well, briefly: **open this chat on a computer with the Whiteboard beside it, and send photos of handwritten working into the same chat from a phone.** Chats sync across devices, so the phone and computer share one conversation. A phone alone also works: answers by typing or photos, with the board shown as a link.
   - Do they want voice mode for the teaching part? If yes, explain the rhythm: start each session in text chat by saying something like "study time"; switch to voice once the board is ready; **switch back to text chat and say "done" at the end**, so the session gets recorded. If they leave without that last step, the next session catches up first.
3. **Create the docs** (templates below) in one go, once you know the first subject. Open the Whiteboard for them. Give each doc a one-line description of what it's for. Tell them they never need to fill anything in themselves: the Tracker and logs are Claude's records, and theirs to read whenever they like. The Teaching Notes are the one place where their own asks about how to be taught live; they can tell Claude these any time.
4. **Save the links** so every future session finds them. Propose a skill edit (the propose_skills tool) that replaces the section 7 placeholders with the real links, doc ids and a one-line "About me" in their words. Tell them to save the card: it's how the system remembers where everything is. If memory is on, also save the links to memory as a backup. If neither works, give them the four links and ask them to keep them.
5. **Map the first subject's syllabus** (section 1 of SKILL.md). Ask for the syllabus document or past papers (or, with no syllabus, any course outline, book or material they're following) if search can't find them; offer to save any PDF they attach as an extract so they never re-attach it. Then write the plan in a line or two: phases, and roughly which days go to which.
6. **Start the first lesson**, or stop here if they'd rather start fresh later. Either way, end setup with the one habit that matters most: *start every session in text chat by saying "study time", and end it by saying "done".*

Over the first two or three sessions, explain the rest only when it comes up: the board's Archive tabs (old sessions to look back at), the Teaching Notes (they can say "remember that I…" any time), and that the tutor may ask them now and then whether a teaching approach is working.

## Doc templates

Create each with the Claude Docs connector. Keep the headings; leave sections empty rather than inventing content. Use the learner's name only if they give it.

**Teaching Notes** (one tab)
- Title "How I Learn — Teaching Notes", byline (date · learner), one line: "What's specific to me. The teaching method itself lives in the teach-me skill."
- Sections: Experiment up next · Context (level, exams and dates, devices, calculator or tools allowed) · How to teach me (their explicit asks) · What lands · What doesn't · Tells and habits · Misconceptions to watch (table: Date | Topic | What I thought | Check / fix, newest first) · Open questions · How this doc stays current (one line: learner-specific only, dated, trimmed as it ages).

**Knowledge Tracker**
- Tabs: Overview (exams with dates, the levels key from section 4, links to the other docs) · one tab per subject · Session log (table: Date | Subject | What we did | Solo / asked | Notes, newest first).
- Subject tab: "Current state" (bullets: course and syllabus version, exams, phase, plan, next up, warm-up items, not exam-ready) · Skills (table: Skill | Syllabus dot point | Past-paper frequency | Level | Last studied | Evidence) · Past-paper progress · Needs revision (bullets).

**Psychology Log**
- Tabs: Overview (what this log is, one paragraph) · Profile (Traits table: Trait | Evidence | How to use it; Candidates table: Candidate | Evidence | Test) · Experiments (Active and queued table: ID | Hypothesis | Move to try | What to watch | Status | Runs | Finding; then Ideas, not yet queued; then Finished) · Method gaps (table: Gap | Where it showed | In the skill?) · Session log (compressed rows) · Full session notes (verbose rows, table with a "Date" header column).
- Seed one or two Queued experiments from the setup conversation if anything stood out (e.g. "learns faster from a worked example first than cold": test both ways); otherwise leave it empty. It fills itself from the first session.

**Whiteboard**
- Tabs: one live tab per subject ("<Subject>": heading, "Board" with "Newest step at the bottom. Answer in chat.", a divider, "Working on", free space, a divider, "How Claude uses this": one line pointing to the skill) · an "Archive" tab, empty, for past session boards.

**Past-paper library** (made per subject, only when the first paper is extracted): a table of Paper | Year | Extract link | Marking guide, plus a line on where the originals came from.
