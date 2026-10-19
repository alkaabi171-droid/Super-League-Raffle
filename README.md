# September Super Team League Raffle Draw

Browser-based raffle webpage for drawing winners from an uploaded Excel or CSV list.

## Features

- Upload participant names from `.xlsx`, `.xls`, `.xlsm`, `.xlsb`, or `.csv`
- Paste names directly, one per line, or paste columns copied from Excel
- Upload or paste previous-month winners to exclude them from the current draw
- Match previous winners by badge number or normalized name
- Support up to 800 unique participants
- Read participant details from `Badge No`, `Name`, and `Title`
- Show the full uploaded list in a visible scrollable table
- Draw 1 unique winner or 10 unique winners at once
- Prevent repeat winners until the raffle is reset
- Highlight the latest winners clearly
- Keep a full draw history with timestamps
- Download all winners as CSV
- Responsive layout for desktop and mobile
- Ready to publish as a static GitHub Pages site

## File Format

- The app reads the first worksheet in the uploaded file.
- Preferred columns are `Badge No`, `Name`, and `Title`.
- Column matching is flexible, so common header variations such as `Badge Number`, `Full Name`, and `Job Title` also work.
- If headers are missing, the app falls back to the first filled cells in each row.
- Duplicate participants are removed automatically.
- If `Badge No` exists, it is used as the unique key. Otherwise the app falls back to `Name + Title`.

## Monthly Fairness Rule

After loading the current month's participant list, use **Exclude Previous Winners** to upload or paste the winners from earlier months. A participant is excluded when their badge number or name matches a previous winner. The exclusion remains active when the raffle is reset and can be replaced by loading a new previous-winners list.

## Run Locally

Open `index.html` in any modern browser.

## Suggested Test Data

You can use the included `sample-participants.csv` file or create a sheet with columns like this:

| Badge No | Name | Title |
| --- | --- | --- |
| 1001 | Ahmed Ali | Sales Executive |
| 1002 | Fatima Saeed | Team Leader |
| 1003 | Noor Hassan | Operations Coordinator |

Pages redeploy refresh.
