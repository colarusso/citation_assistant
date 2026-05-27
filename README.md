# Citation Tool Test (static-file web app)

You can learn more about why this exists here: [Algos, bias, due process, & you](https://suffolklitlab.org/algos-bias-due-process-you/). 

If you want to play around, here's a [live version](https://www.davidcolarusso.com/42/citation_assistant/), and of course, you can download, edit, and run this locally. 

## What this is
A single-page, client-only web simulation designed to teach *automation bias / automation misuse* in a legal citation-checking context.

- No backend.
- No database.
- All data stays in the browser (localStorage).
- Export results as JSON at the end.

All authorities/cases are **fictionalized** for teaching purposes.

## Instructor tips
- Ask students to export JSON at the end and submit to LMS/email.
- The app is tuned for a ~20 minute session with phased manipulation:
  Phase 1: very reliable assistant
  Phase 2: competition pressure increases
  Phase 3: domain shift (authority weight / jurisdiction)
- You can have studets download their results as a `.json` file and share it with you. You can then drag and drop these files into the dashboard tool (available at `dashboard/index.html`) to look at the results

## Quality checks
Open `check.html` (served via a local server) to review and edit `items.json`, then export a new `items.json`.

Append a `#test` to the `index.html` page to turn on output in the browser’s console log. This is intended to help perform quality checks of the assistant in use and confirm expected behavior (i.e., it let your see what the tool considers ground truth so you can compare it with the on-screen output). 
