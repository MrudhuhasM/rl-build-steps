# RL build steps

The sections of each chapter of the RL build (the book in the RL Roadmap doc), one file per
chapter in `steps/`. The time log on the spare laptop reads this repo: **Import from GitHub**
pulls it and adds any sections it doesn't have yet.

A chapter's file is added when that chapter opens, so only the chapters reached so far are here.

## Format

`steps/chapter-N.txt`: a heading line for the chapter, then one line per section. A
`question:` line under the heading and a `why:` line under each section are optional, and the
time log shows them beside the section, so you can always see what a section is for.

```
Chapter 1 — The Whole Loop, Crudely: your first model that learns from reward
question: How does a model get better from nothing but a score?

1.1 A math verifier
why: RL needs a score it can trust before anything can learn.

1.2 REINFORCE, then GRPO
why: …
```

- **Heading:** `Chapter N — Name`. A dash, en dash or colon after the number all work.
- **Sections:** `N.M Section name`. The number before the dot is the chapter and the one after
  it is the section. The number is the section's identity: the time log matches sections by
  it, so never renumber a section that already has time tracked against it.
- **`question:`** goes after the heading; **`why:`** goes after its section, before the next one.
- Blank lines are ignored, and so are other lines, so a note to yourself is fine as long as it
  doesn't start with a number (`1. …` or `1) …` is read as section 1 of the chapter above it).

## Changing a chapter

- **New chapter:** add `steps/chapter-N.txt`, push, then click **Import from GitHub**.
- **Rename a section or change its why:** edit the text and keep the number. The time log
  takes the new text and keeps the section's times.
- **Add a section in the middle:** give it the next free number (for example `1.9`), even if it
  sits between 1.3 and 1.4 in the file. The time log lists sections by number.
- **Remove a section:** deleting a line doesn't remove it from the time log. Use **Delete**
  there; it only works on sections that haven't been started.
- **Starting the whole book again:** **Start over…** in the time log clears everything and
  reloads Chapter 0.
