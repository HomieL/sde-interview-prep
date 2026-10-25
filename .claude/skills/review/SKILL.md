---
name: review
description: Review a coding-interview solution I wrote. Use when I say /review, "check my solution", or point at a file in solutions/. Argument is a file path or problem name.
---

# Solution review

1. Read the file. If the problem statement isn't in it, ask me for it.
2. Write a test file next to it (`solutions/test_<name>.py`) with normal cases and
   edge cases: empty input, single element, duplicates, negatives, large input
   for timing. Run it and report results.
3. Check my stated complexity. If I didn't state one, ask me before telling me.
4. Review like an interviewer, in this order:
   - Correctness bugs (with the failing input)
   - Complexity: is there a better approach? Give a hint level first, not the answer.
   - Code clarity: naming, unnecessary branches, helper functions
   - What I should have said out loud while writing it
5. Only if I ask, show a cleaner version, keeping my approach where possible.
6. Log the attempt in `progress/log.md` and update `progress/weak-spots.md`.
