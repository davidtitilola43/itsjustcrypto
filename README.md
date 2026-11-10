# Its Just Crypto

Crypto news, minus the noise: hacks, new laws, politics and market moves, explained in plain English for students, young professionals, accountants and anyone curious about digital assets.

Live site: **[itsjustcrypto.com](https://itsjustcrypto.com)**

## What it is

A weekly, community-focused roundup of what is moving crypto. The page includes:

- a lead story and a "week in numbers" strip
- a story feed you can filter by topic (Politics, New laws, Markets, Hacks, For accountants), where each story ends with a **Why it matters to you** note and source links
- a to-scale chart of the year's biggest hacks
- a short glossary of the week's jargon, a quiz, and a "Coming up" diary
- links to join the community on Substack, Instagram and LinkedIn

## Project structure

| File         | Purpose                                                            |
| ------------ | ------------------------------------------------------------------ |
| `index.html` | The whole site: markup, styles and script in one self-contained file |
| `CNAME`      | Custom domain for GitHub Pages (`itsjustcrypto.com`)               |

There is no build step. The site is served directly by GitHub Pages from the `main` branch.

## Adding a new story

1. Open `index.html` and copy an existing `<article class="card" ...>` block inside `#feed`.
2. Set `data-t` to `politics`, `laws`, `markets`, `hacks` or `acct`, and use the matching `tag` class.
3. Fill in the headline, short summary, full text, *Why it matters to you* note, date and source links.
4. Update the week in the hero (`Week of ...`) and the numbers strip if needed.
5. Commit to `main`. GitHub Pages redeploys automatically.

To preview locally, open `index.html` in a browser, or run `python3 -m http.server` and visit `http://localhost:8000`.

## Disclaimer

This is a personal project, kept as a working reference rather than professional advice. Always check the primary sources ([IASB](https://www.ifrs.org), [FASB](https://www.fasb.org), [AICPA](https://www.aicpa-cima.com)) before relying on anything here. Nothing on the site is financial advice. Views are the author's own and do not represent the position of any current or former employer.
