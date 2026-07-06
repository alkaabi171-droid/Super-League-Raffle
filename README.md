# Super League Raffle

Browser-based raffle webpage for drawing winners from an uploaded Excel or CSV list.

## Features

- Upload participant names from .xlsx, .xls, or .csv
- Keep up to 50 unique names
- Show the full uploaded list in a visible scrollable table
- Draw 10 unique winners at once
- Prevent repeat winners until the raffle is reset
- Highlight the latest 10 winners
- Keep a full draw history with timestamps
- Download all winners as CSV
- Responsive layout for desktop and mobile
- Ready to publish as a static GitHub Pages site

## File Format

- The app reads the first worksheet in the uploaded file.
- It uses the first non-empty cell in each row as the participant name.
- Common headers such as Name, Names, Participant, Participant Name, and Employee Name are ignored automatically.
- Duplicate names are removed automatically.

## Run Locally

Open index.html in any modern browser.

## Publish To GitHub Pages

1. Create a GitHub repository named Super-League-Raffle.
2. Upload the project files to the repository root.
3. Open the repository settings on GitHub.
4. In Pages, choose Deploy from a branch.
5. Select the main branch and the / (root) folder.
6. Save the settings and wait for GitHub Pages to publish the site.

## Suggested Test Data

You can use the included sample-participants.csv file or create a sheet with one column like this:

| Name |
| --- |
| Ahmed Ali |
| Fatima Saeed |
| Noor Hassan |

Triggering GitHub Pages redeploy.
