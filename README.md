# The Supervisor's Field Kit

Free printable companion sheets for readers of *Run the Shift: The Warehouse
Supervisor's Field Guide* by Nicola Duma.

**→ [nicola-duma.github.io/run-the-shift](https://nicola-duma.github.io/run-the-shift/)**

No sign-up, no email required.

## What's in the kit

Three sheets, each in two paper sizes:

| Sheet | Use it | Letter | Tabloid |
|---|---|---|---|
| **Shift Handover Sheet** | Every shift | 8.5 × 11″ | 11 × 17″ |
| **Weekly Floor Planner** | Every week | 11 × 8.5″ | 17 × 11″ |
| **52 Toolbox Talk Topics** | Once — lasts a year | 8.5 × 11″ | 11 × 17″ |

The sheets are built around the numbers in the book — the UPH scale, the
dock-to-stock window, the corrective-action clocks, the Perfect Order Rate
calculation — so they make more sense with the book open beside them.

**Letter is the primary size.** It is the one that prints in any American office.
Tabloid is there for whoever has the large-format printer. There is deliberately no
A3: 297 × 420 mm is not a size a US office keeps in stock, and a supervisor who
sends A3 to the shift lead's printer gets a scaled page with the margins cut off.

## Repository layout

```
index.html   landing page, served by GitHub Pages
*.pdf        the six sheets
```

That is the whole repo. It is a static site with no build step — GitHub Pages
serves `index.html` from the default branch.

## Regenerating the sheets

The PDFs are generated, not drawn by hand. The build scripts live with the book's
manuscript sources and are **not** part of this repository, which holds only the
published output.

Two things worth knowing before replacing a PDF here:

- The three sheets share one module for header, palette, rules, boxes and footer.
  Regenerate all six together, so the kit keeps looking like it came out of the
  same book.
- The download URL printed in each sheet's footer comes from a **single shared
  constant**. Change it in one place and re-export; that way no sheet can be left
  carrying an old link. This matters more than usual — a URL printed on paper
  cannot be corrected after the fact.

Point readers at the page, never at the PDFs directly, so the sheets can be
updated without breaking a link that is already in print.

## License

The sheets and this page are released under
**[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)**
(Attribution-NonCommercial-NoDerivatives). Full legal code in [`LICENSE`](LICENSE).

In plain terms: download them, print them, hand them around the shift, photograph a
sheet and send it to your leads — all of that is fine, and it is the point. Keep the
credit line and the footer. Do not sell them, and do not publish a changed version.

"NonCommercial" is aimed at resale and repackaging, not at you: printing a sheet and
using it to run your shift is exactly what it was made for, whoever signs your
paycheck.

© 2026 Nicola Duma.

## Disclaimer

These are personal working sheets, **not facility records**. They do not replace
your site's own forms, logs, or safety program, and nothing here is legal or
safety-engineering advice. Confirm anything you intend to write into a procedure
with your own EHS professional. In an emergency, call 911.
