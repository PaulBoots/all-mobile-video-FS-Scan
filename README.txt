All Mobile Video v46 — OneDrive Auto Update

Configured for:
GitHub Pages:
https://paulboots.github.io/all-mobile-video-FS-Scan/

Microsoft Application (client) ID:
fb3d7e2e-4a4a-48e0-af82-824c614ace4c

AMV OneDrive / SharePoint folder:
JOBS

NEW:
- CONNECT ONEDRIVE
- LOAD ONEDRIVE JOB
- SAVE NOW
- AUTO UPDATE EXCEL checkbox
- OneDrive status shows CONNECTING / SAVING / SAVED / ERROR
- After connection, job changes automatically update the Excel .xlsx file in the JOBS folder.
- Uses a short delay after changes so it does not upload on every single keystroke.
- Scan OUT, Scan IN, notes, delete, undo, job information, truck, checker, and completion changes trigger cloud autosave.
- Existing OneDrive Excel jobs can be opened in the app.
- Individual Scan History DELETE button fixed.

Cloud Excel filename:
All-Mobile-Video-[JOB NUMBER].xlsx

IMPORTANT:
1. Upload the new index.html and amv-logo.jpg to the SAME GitHub repository.
2. Open the GitHub Pages HTTPS site.
3. Click CONNECT ONEDRIVE.
4. Sign in to the AMV Microsoft account that has access to the JOBS folder.
5. Accept the requested Microsoft permissions if prompted.
6. After connection, status should show CONNECTED — AUTOSAVE READY.
7. Enter Job Name and Job Number. Auto cloud saving starts when both are present.

No Microsoft password or client secret is stored in this app.
Authentication uses OAuth authorization code + PKCE.

If an Excel file is open in desktop Excel at the same time, OneDrive may take a moment
to sync the newly uploaded version and Excel may display a refresh/conflict notification.
