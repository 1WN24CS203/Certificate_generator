# Gatherwell Event Survey & Certificate Portal

A standalone, responsive event survey and certificate portal. Open `index.html` in a browser to use the organizer studio. Share the event-specific participant URL from the studio to open the participant portal.

## Features

- Manage events, survey links, verification settings, certificate templates, and participant logs in the organizer studio.
- Verify participants with a survey link and dwell timer, a completion code, or both.
- Design certificates and download personalized PNG or print-ready PDF files.
- Export participant claims to CSV.

## Local data and deployment

This is a static, single-file app. Event settings, uploaded templates, verification codes, and participant logs are stored in the browser's `localStorage`. That means each browser/device has its own data: deploying the page does not synchronize organizer data with participants. To share event data across devices or securely verify survey completion, connect the app to a backend and enforce verification there.

The page uses Tailwind CSS and jsPDF from CDNs, so those features require an internet connection.

## Deploy to Vercel

Import this repository into Vercel and deploy it as a static site. The `index.html` file is at the repository root, so no build command is needed.
