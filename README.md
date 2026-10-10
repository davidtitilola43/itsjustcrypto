# Its Just Crypto

A running record of what the **IASB**, **FASB** and **AICPA** are doing about crypto and digital asset accounting, written in plain terms.

Live site: **[itsjustcrypto.com](https://itsjustcrypto.com)**

## What it is

Standard-setters move slowly and in fragments: a meeting paper here, a practice aid update there. This site collects the developments that matter to anyone accounting for or auditing digital assets. Each entry covers what changed, who changed it, and why it matters for the work. There are no hot takes and no price talk.

Each entry includes:

- the standard-setter (IASB, FASB or AICPA) and the date
- its status, such as *research stage*, *deliberations underway* or *in force*
- a short summary of the development
- a **Why it matters** note for practitioners
- a link to the primary or secondary source

You can filter entries by standard-setter, expand them one at a time or all at once, and copy a direct link to any entry.

## Project structure

| File         | Purpose                                                            |
| ------------ | ------------------------------------------------------------------ |
| `index.html` | The whole site: markup, styles and script in one self-contained file |
| `CNAME`      | Custom domain for GitHub Pages (`itsjustcrypto.com`)               |

There is no build step. The site is served directly by GitHub Pages from the `main` branch.

## Adding a new development

1. Open `index.html` and copy an existing `<article class="entry" ...>` block.
2. Set `data-body` to `iasb`, `fasb` or `aicpa`, and give the entry a unique `id` (for example `entry-05`). Update the matching `aria-controls` / panel `id`.
3. Fill in the date, status, title, summary, *Why it matters* note and source link.
4. Update the `UPDATED` date in the masthead (`#last-updated`).
5. Commit to `main`. GitHub Pages redeploys automatically.

To preview locally, open `index.html` in a browser, or run `python3 -m http.server` and visit `http://localhost:8000`.

## Disclaimer

This is a personal project, kept as a working reference rather than professional advice. Always check the primary sources ([IASB](https://www.ifrs.org), [FASB](https://www.fasb.org), [AICPA](https://www.aicpa-cima.com)) before relying on anything here for client work. Views are the author's own and do not represent the position of any current or former employer.
