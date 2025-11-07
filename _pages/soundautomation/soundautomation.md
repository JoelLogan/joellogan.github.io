---
title:
layout: default
permalink: /soundautomation
published: true
---

## Joel's Sound Automation

Joel's Sound Automation is a personal, automated script designed to process scheduling files within a specific Google Drive folder. It is not a public application and is intended only for the developer's use.

What It Does
This script runs automatically to perform a 3-part "convert and clean" workflow:

1. Finds Excel Files: It monitors a specific Google Drive folder for any new schedules uploaded as .xls or .xlsx files.

2. Converts & Cleans: For each Excel file, it:

    - Creates a new Google Sheet file.

    - Opens the new Google Sheet and automatically deletes any rows that contain strikethrough text.

    - Moves the original Excel file to the trash.

3. Logs the Job: It appends a new row to a central "index" spreadsheet, logging the name and file ID of the new, clean Google Sheet for use in other automations.

### Why This Script Needs Google Permissions
This is a non-interactive, automated script, so it cannot ask for file-by-file permission using a file picker. To perform its job, it requires one-time authorization for the following:

- Google Drive Access (.../auth/drive): This is required to read the original Excel files, create the new Google Sheet files, and move the original Excel files to the trash.

- Google Sheets Access (.../auth/spreadsheets): This is required to write a log entry to the "index" sheet and to open, read formatting from, and delete rows in the newly created Google Sheets.

This script only accesses files and data within the developer's own account.

### Privacy
Your privacy is important. This script does not store, share, or access any data outside of its core functions listed above.

[View the full Privacy Policy here](https://joellogan.com/soundautomationprivacy)