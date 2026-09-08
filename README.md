# UASAM 2026 — conference website

Website for **The 38th Annual University of Alabama System Applied Mathematics Meeting**,
Saturday, November 7, 2026, The University of Alabama, Tuscaloosa.

Live site: https://jiazhaomath.github.io/UASAM2026/

## What is here

| File | Purpose |
|---|---|
| `index.html` | The 2026 meeting: schedule, call for talks, venue, organizers |
| `previous-meetings.html` | Programs and abstracts of past meetings (2025 so far); add a section per year |
| `style.css` | Hand-written stylesheet. No frameworks, no external fonts or scripts |
| `assets/38th_Applied_Math_Meeting_Schedule.pdf` | Tentative schedule (built from the `.tex` in the parent folder) |
| `assets/37thAppliedMathMeeting_UAH.pdf` | 2025 program and abstracts |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Before announcing: fields still marked TBD

Search `index.html` for `tbd`. Each placeholder is a yellow `<span class="tbd">…</span>`
with an HTML comment next to it saying what to put there.

1. The nine talk slots in the schedule table. Replace each `Faculty Talk n` /
   `Student Talk n` cell with `Speaker Name (Campus) — Talk title` and drop `class="slot"`.

When the schedule is final, change the heading "Tentative schedule" to "Schedule" and
rebuild the PDF in `assets/` from `../38th_Applied_Math_Meeting_Schedule.tex`.

## Editing and publishing

Edit `index.html` in any text editor, then:

```sh
git add -A
git commit -m "Update schedule"
git push
```

GitHub Pages redeploys from the `main` branch root within about a minute.
To preview locally, open `index.html` in a browser; nothing needs to be built.
