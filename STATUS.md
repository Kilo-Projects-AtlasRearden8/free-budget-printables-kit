# STATUS

## What was built

Free Budget Printables Kit — a set of fillable, printable, large-print friendly budget printables from Asdale Dynamics, LLC. No account needed; everything runs locally in the browser, nothing is saved or sent anywhere.

Files:
- `index.html` — kit landing page with links to all sheets and usage instructions
- `monthly-budget-planner.html` — income vs. expenses by category, planned vs. actual, variance
- `expense-tracker.html` — log purchases by date, category, amount with monthly totals
- `bill-calendar.html` — monthly calendar to mark bill due dates and check off paid bills
- `savings-goal-sheet.html` — set a target, track contributions, progress bar, remaining
- `assets/style.css` — shared styles (screen + print), large-print friendly
- `README.md` — kit description, how to use, About, license
- `LICENSE` — MIT License, copyright line: `Copyright (c) 2026 Asdale Dynamics, LLC`
- `STATUS.md` — this file

## How to run

Open any `.html` file directly in a browser (Chrome, Edge, Safari, Firefox). No build step, no install, no server needed.

- To use on screen: open the file and fill in the form fields.
- To print: press `Ctrl+P` / `Cmd+P`. Print styles hide buttons/controls and output high-contrast black-on-white.
- All four sheets link back to `index.html` via a "Back to kit" button and each has a "Print this sheet" button.

## Verification results

- All five HTML files parse cleanly (no unclosed tags, no structural errors) — verified with Python `html.parser`.
- `LICENSE` contains the exact copyright line: `Copyright (c) 2026 Asdale Dynamics, LLC`.
- `Asdale Dynamics, LLC` credited in `README.md` and in every HTML page (title, footer, About link to dylanasdale.github.io).
- No secrets, API keys, or personal data found in any file.
- No `.github/workflows` files present.
- No remote repo configured; nothing pushed or published.

## Known gaps

- Sheets are static HTML with no client-side calculation (totals display `$0.00` placeholders); intended as printable worksheets to fill by hand or on screen.
- No automated test suite or CI config (none requested; no `.github/workflows` added).
- Bill calendar day numbers are blank inputs to fill in manually (no JS to auto-generate a calendar grid), keeping it dependency-free and print-first.
