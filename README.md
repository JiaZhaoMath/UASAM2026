# UASAM 2026 — conference website

Website for **The 38th Annual University of Alabama System Applied Mathematics Meeting**,
Saturday, November 7, 2026, The University of Alabama, Tuscaloosa.

Live site: https://jiazhaomath.github.io/UASAM2026/

## What is here

| File | Purpose |
|---|---|
| `index.html` | The 2026 meeting: schedule, venue, organizers (call for talks commented out) |
| `previous-meetings.html` | 2025 program and abstracts. Kept in the repo but **not linked** from `index.html`; re-add the nav entry there to publish it |
| `style.css` | Hand-written stylesheet. No frameworks, no external fonts or scripts |
| `abstracts/*.md` | One Markdown record per talk (speaker, campus, role, title, abstract); the source for the schedule cells. See `abstracts/README.md` |
| `assets/38th_Applied_Math_Meeting_Schedule.pdf` | Tentative schedule (built from the `.tex` in the parent folder) |
| `assets/37thAppliedMathMeeting_UAH.pdf` | 2025 program and abstracts |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Before announcing: fields still open

All nine speakers are on the page (3 faculty, 6 students), each with a title and abstract.
Still open:

1. The welcome-remarks speaker, currently shown as "Welcome remarks (to be announced)".
   Replace the parenthetical with the speaker, following the 2025 form: `Welcome remarks by
   Department Chair Dr. Name`.

Mirror every schedule change in `../38th_Applied_Math_Meeting_Schedule.tex`, rebuild with
`latexmk -pdf -g` (plain `latexmk` may report "Nothing to do"), and copy the PDF to `assets/`.
When the schedule is final, change the heading "Tentative schedule" to "Schedule".

## Editing and publishing

Edit `index.html` in any text editor, then:

```sh
git add -A
git commit -m "Update schedule"
git push
```

GitHub Pages redeploys from the `main` branch root within about a minute.
To preview locally, open `index.html` in a browser; nothing needs to be built.
