# Interview coach for Claude Code

## Setup (once)
1. Install Claude Code (see https://code.claude.com/docs).
2. Unzip this folder somewhere, e.g. `~/interview-coach`.
3. Open `progress/log.md` and fill in your interview dates.
4. Optional but recommended: put it on GitHub and turn on Pages (below).

## Each session
    cd ~/interview-coach
    claude

Then type one of:
- `/plan` what to practice today
- `/mock` a timed 45-minute mock round (`/mock graphs` for a topic)
- `/review solutions/2026-10-25-some-problem.py` feedback on your own attempt
- `/stories` behavioral and project practice
- `/add-problem 1239` write up a solved problem on your site

## Your cheat sheet site
The whole site is `docs/index.html`. Open it in a browser to use it offline.

To host it with GitHub Pages:

    git init
    git add .
    git commit -m "first commit"
    # create an empty repo on github.com, then:
    git remote add origin https://github.com/<you>/interview-coach.git
    git branch -M main
    git push -u origin main

On GitHub: Settings → Pages → Deploy from a branch → `main` / `/docs` → Save.
The site appears at `https://<you>.github.io/interview-coach/` within a few minutes.
After that, every `git push` updates it.

A private repo with Pages normally needs a paid plan; the GitHub Student
Developer Pack may cover it. Otherwise keep the repo public, or move your
`solutions/` and `progress/` into a separate private repo.

## Tips
- Code mocks in a plain editor with autocomplete off, since that's closer to the real thing.
- Talk out loud during mocks, even alone. Type your reasoning as comments if you can't.
- Edit CLAUDE.md whenever the coach does something you don't like twice.
