# Talk records for the 38th meeting (November 7, 2026)

One Markdown file per talk, named `<campus>-<speaker>.md`. These files are the editable
record of the program; `../index.html` and `../../38th_Applied_Math_Meeting_Schedule.tex`
are rendered from them by hand. GitHub Pages serves this repo as-is (`.nojekyll`), so these
files are readable on GitHub but are not pages on the live site.

## Front matter

```yaml
---
speaker: Full Name
prefix: Dr.            # faculty only; omit for students
role: faculty          # faculty | student
campus: University of Alabama at Birmingham   # as written on the 2025 page
campus_short: UAB      # UA | UAB | UAH
title: Talk title      # quote it if it contains a colon
slot: 10:50–11:30 a.m. # the row in the schedule table
coauthors: [Name, Name]  # only when the abstract lists them
source: ../../abstracts/<original file>       # where the text came from
---
```

The body is the abstract, verbatim from the speaker, with only typography normalised
(en dashes, Unicode math such as `ℝ^d`, `O(h^k + Δt^2)`). Coauthors are not shown on the
speaker line; a closing sentence "This is joint work with …" ends the abstract instead.

## Program order (decided 2026-10-17)

Morning, faculty (40 min): UA, UAB, UAH.
Afternoon, students (20 min), host campus (UA) last in each block:
1:30 UAB, 1:50 UAH, 2:10 UA; 3:00 UAB, 3:20 UAH, 3:40 UA.

## Open slots

No speaker slots are open. One speaker is confirmed with title and abstract pending:
Robert Stephens (UAH, 3:20–3:40 p.m., `uah-stephens.md`).

## Adding a talk

1. Write the `.md` file here.
2. In `../index.html`, replace the matching `<td class="slot">…</td>` with the cell
   markup used by the other talks (title span, speaker span, `<details>` abstract).
3. Update the same row in `../../38th_Applied_Math_Meeting_Schedule.tex`, rebuild with
   `latexmk -pdf -g`, copy the PDF to `../assets/`.
4. Bump the `?v=` on the stylesheet links only if `style.css` changed; update the footer date.
