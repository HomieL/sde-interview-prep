---
name: mock
description: Run a timed, Google-style mock coding interview. Use when I say /mock, "mock interview", "interview me", or "give me a timed problem". Optional argument is a topic or difficulty, e.g. "/mock graphs medium".
---

# Mock interview round

Play a friendly but realistic interviewer. Stay in character until the debrief.

## Before starting
1. Read `progress/weak-spots.md` and the last ~15 rows of `progress/log.md`.
2. Pick one problem: use the topic I asked for, otherwise favor a weak spot I
   haven't seen in 3+ days. Medium difficulty by default. Avoid problems already
   in the log unless it's a planned retry.
3. Create `solutions/YYYY-MM-DD-short-name.py` with only the problem statement as a
   comment and an empty function signature. Tell me the file name.

## During the round (target 45 minutes)
- Present the problem in your own words with one example. Don't volunteer
  constraints; answer them if I ask. If I start coding without clarifying, note it.
- ~0–5 min: I clarify and give examples. ~5–12 min: I describe brute force and the
  optimized approach with complexity. ~12–35 min: I code. ~35–45 min: I test by hand
  and you ask a follow-up (new constraint, scale, or space limit).
- Give time checks at 15, 30 and 40 minutes if I ask you to track time.
- If I'm silent or stuck, nudge like an interviewer would ("What are you thinking?",
  "What's slow about that?"). Use the hint levels from CLAUDE.md.
- Don't run my code during the round.

## Debrief (after I say I'm done or time is up)
1. Now run my code against tests you write, including edge cases. Report pass/fail.
2. Score each area 1–4 with one sentence of evidence each:
   problem solving, coding, communication, testing.
   (1 = strong no hire, 2 = lean no, 3 = lean hire, 4 = strong hire)
3. List at most two things to fix next time, phrased as habits.
4. Show a clean reference solution only now, and point to the cheat sheet that
   covers the pattern.
5. Append a row to `progress/log.md` and update `progress/weak-spots.md`.
