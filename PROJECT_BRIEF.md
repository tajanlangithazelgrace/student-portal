# One-Page Project Brief

## Project title
**Barangay Peace & Order — Incident Blotter Tracker**

## Pitch
A simple one-page web app prototype that helps a barangay peace-and-order desk demonstrate how incoming community concerns can be recorded in one list and tracked from receipt to review or resolution.

## Community problem
Community concerns may be received verbally, by phone, or through handwritten notes. When reports are kept in different places, it can be difficult for desk staff to find a previous report or determine its follow-up status. The project demonstrates a basic, organized record list for sample reports.

## Target users
- **Primary:** Barangay peace-and-order desk staff who receive and follow up on reports.
- **Secondary:** Residents who raise community concerns. Residents are not given direct app accounts in this lab scope; their reports are represented using fictional data only.

## Feature scope (FR-01)
**Record and track a sample incident report.** A staff user can enter a report date, incident category, general location/purok, and a short neutral summary. The app creates a reference ID and starts the report at Received. Staff can search/filter reports and update a report to Under Review or Resolved.

## Acceptance criteria
1. A valid report is saved with an ID and Received status and appears in the report list.
2. Search and status filtering show only the matching reports.
3. A status change is saved and remains after a page refresh.

## Out of scope
Real incident processing, police case management, resident accounts, logins, role permissions, file/photo uploads, SMS/email notifications, a live database, and multi-device synchronization. These are deliberately excluded to keep the lab app small.

## Architecture
One `index.html` file contains the page structure, styles, and vanilla JavaScript. The browser validates inputs, creates report objects, renders the list, and stores the demo records in `localStorage`. There is no backend or external service.

## Privacy and safety note
Use only made-up examples. Do not enter actual names, phone numbers, exact home addresses, sensitive personal information, or details of real cases. `localStorage` is not secure storage and this prototype is not for official records.
