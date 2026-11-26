# RL build steps

The step list for each phase of the RL build, one file per phase in `steps/`.
The time log on the spare laptop reads this repo: **Import from GitHub** pulls it and
adds any steps it doesn't have yet.

## Format

`steps/phase-N.txt`: one heading line for the phase, then one line per step.

```
Phase 1 — Thin slice: the whole loop, crude
1.1 Environment interface
1.2 Math verifier
1.3 REINFORCE with a baseline
```

- **Heading:** `Phase N — Name`. A dash, en dash or colon after the number all work.
- **Steps:** `N.M Step name`. The number before the dot is the phase and the one after it is
  the step. The number is the step's identity: the time log matches steps by it, so never
  renumber a step that already has time tracked against it.
- Blank lines are ignored, and so are other lines, so a note to yourself is fine as long as it
  doesn't start with a number (`1. …` or `1) …` is read as step 1 of the phase above it).

## Changing a phase

- **New phase:** add `steps/phase-N.txt`, push, then click **Import from GitHub**.
- **Rename a step:** edit its name and keep its number. The time log takes the new name and
  keeps the step's times.
- **Add a step in the middle:** give it the next free number (for example `1.9`), even if it sits
  between 1.3 and 1.4 in the file. The time log lists steps by number.
- **Remove a step:** deleting a line doesn't remove the step from the time log. Use **Delete**
  there; it only works on steps that haven't been started.
