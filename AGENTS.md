# AGENTS.md

## What this repo is
Collection of static HTML/CSS course assignments ("tugas") plus extra exercises. **No build system, no package manager, no tests, no lint/format config, no CI.** Do not invent `npm`/`make` commands.

## Run / verify
Files are opened directly in a browser — there is nothing to compile. For a local check:
`python3 -m http.server` from the assignment folder, then open `index.html` / `tugas*.html`.
There is no automated way to verify changes; inspect the HTML/CSS.

## Layout
Each folder is an independent assignment with its own entry HTML and CSS. Relative asset paths differ per folder — keep them consistent when editing.
- `tugas1/tugas1.html` — inline/none; basic HTML (intentionally uses deprecated tags/attrs)
- `tugas2/index.html` — CSS in `styles/style.css`, image in `images/profile.jpg`
- `tugas3/tugas-css1.html` — CSS is inline in `<head>`
- `tugas4/tugas-css2.html` — CSS in `css/style.css`
- `web-css/index.html` — CSS in `css/style.css`, assets via `css/`
- `web-bootstrap/index.html` — inline `<style>` + Bootstrap 5.3.8 from CDN (SRI hashes present)

## Gotchas
- Content is written in Indonesian (`lang="id"` or `"en"`); match the existing language when editing copy.
- `tugas3/style.css` is empty and unused — edit the inline `<style>` block, not that file.
- `tugas1` deliberately uses old HTML (`bgcolor`, `<marquee>`, `<font>`); do not "modernize" it unless asked. It also contains a `<font colour=...>` typo (`colour` is not a valid attribute).
- Comments and some IDs/classes are Indonesian; follow local naming rather than introducing new conventions.
- Repo has no `.gitignore`; avoid committing generated/editor files.
