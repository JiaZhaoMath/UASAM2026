# UASAM 2026 — conference website

Website for **The 38th Annual University of Alabama System Applied Mathematics Meeting**,
Saturday, November 7, 2026, The University of Alabama, Tuscaloosa.

Live site: https://zhaojia.net/UASAM2026/ (since 2026-10-20, when zhaojia.net became the custom domain of
the JiaZhaoMath GitHub Pages user site; the old https://jiazhaomath.github.io/UASAM2026/ redirects there)

## What is here

| File | Purpose |
|---|---|
| `index.html` | The 2026 meeting: schedule, venue, organizers (call for talks commented out) |
| `previous-meetings.html` | Meeting history (1995–2026): overview table of all meetings plus programs where found. Linked from the `index.html` nav as "Past meetings". **Generated** by `../history_sources/build_history_page.py` from `../history_sources/meetings.py` (private folder outside the repo); sources in `../meeting_history.md` |
| `assets/history/` | Archived programs of past meetings (2012, 2013, 2017, 2018, 2019, 2021), copied from department sites / the Internet Archive |
| `style.css` | Hand-written stylesheet. No frameworks, no external fonts or scripts |
| `abstracts/*.md` | One Markdown record per talk (speaker, campus, role, title, abstract); the source for the schedule cells. See `abstracts/README.md` |
| `assets/38th_Applied_Math_Meeting_Schedule.pdf` | Tentative schedule (built from the `.tex` in the parent folder) |
| `assets/37thAppliedMathMeeting_UAH.pdf` | 2025 program and abstracts |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Before announcing: fields still open

All nine speakers are on the page (3 faculty, 6 students), each with a title and abstract.
Still open: none. The welcome row reads just "Welcome remarks" with no speaker named. If a
speaker is named later, follow the 2025 form: `Welcome remarks by Department Chair Dr. Name`.

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
