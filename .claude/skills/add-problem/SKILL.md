---
name: add-problem
description: Add a solved LeetCode problem as a new page in docs/index.html. Use when I say /add-problem, "add this problem to my site", or give a LeetCode number to write up. Argument is the problem number and name, optionally a path to my solution in solutions/.
---

# Add a problem page

The site is one file, `docs/index.html`. Each problem is an `<article>` in the
"LeetCode problems" section. Copy the structure of the existing `lc1239` article.

## Steps
1. If I gave a solution file, read it and use my approach as the main solution.
   Otherwise ask whether I've solved it yet; don't write up a problem I haven't tried.
2. Add a new article just before the `<!-- end problems -->` marker comment (or after
   the last `class="sheet prob"` article if the marker is missing), with:
   - `id="lc<number>"`, `class="sheet prob"`, `data-group="LeetCode problems"`,
     `style="--h:330"`
   - `data-title="<number> · <short title>"`, `data-num`, `data-name`, `data-diff`
     (Easy/Medium/Hard), `data-pattern`, `data-idea` (one line). The Problem log
     table builds itself from these attributes.
3. Sections, in this order: the problem in plain words (paraphrase, never copy the
   LeetCode statement), an example to trace (make up your own), read the constraints,
   key insights, solution code with "how to read it", a trace of the example,
   complexity, common bugs, how to say it in the interview, likely follow-ups, related.
   Link to the matching cheat sheet with `<a href="#sheet-id" data-go="sheet-id">`.
4. Code goes in `<pre>` blocks as plain Python. Escape `<` as `&lt;` when it's
   followed directly by a letter, and `&` as `&amp;`.
5. Test every code block: write a brute-force checker in a scratch file and compare
   on random inputs. Don't add code that fails.
6. Open the page in a browser if one is available, or at least check the HTML parses.
7. Commit with message `add LC <number>` and remind me to `git push` to update the site.
