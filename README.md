# Barangay Peace & Order — Incident Blotter Tracker

A small, one-page community web app prototype for Lab 1. It demonstrates how a barangay peace-and-order desk could record a sample incident report and track its follow-up status.

> **Classroom prototype only. Do not enter real complainant names, contact details, exact addresses, allegations, or actual incident information.** This app stores data in the current browser's `localStorage`. It has no authentication, server, encryption, access control, audit trail, or secure backup and is not suitable for official barangay records.

## Community problem
Small barangay desks may receive concerns through conversations, calls, or handwritten notes. When information is kept in separate places, staff can have difficulty checking whether a report was received, is being reviewed, or has been resolved. This prototype demonstrates a simple, centralized list for sample reports and their statuses.

## FR-01 — Record and track a sample incident report
**User story:** As a barangay peace-and-order desk staff member, I can record an incident report and update its follow-up status, so that community concerns can be organized and their progress can be checked.

### Acceptance criteria
1. Given the report form is open, when the user submits a report with a date, category, general location, and short summary, then the app creates a unique report ID and displays the report with the status **Received**.
2. Given there are saved reports, when the user searches by report ID, category, location, or summary and/or chooses a status filter, then only matching reports are displayed.
3. Given a report exists, when the user changes its status to **Under Review** or **Resolved**, then the updated status and summary counts are saved and remain after refreshing the page.

## Users
- **Primary user:** Barangay peace-and-order desk staff member who records and follows up on incoming concerns.
- **Secondary stakeholder:** Barangay resident who reports a concern (represented only by fictional sample data in this lab prototype).

## Features
- Add a fictional sample report with date, category, general location, and brief summary.
- Generate a report reference ID.
- Search report ID, category, location, and summary.
- Filter reports by Received, Under Review, or Resolved.
- Update a report's status, delete demo records, and reload fictional sample records.
- Save and reload demo records using browser `localStorage`.

## Architecture
- **Frontend:** One `index.html` file containing HTML, CSS, and vanilla JavaScript.
- **Persistence:** Browser `localStorage` under the key `barangayPeaceOrderBlotter_demo_v1`.
- **Backend/API:** None. This is intentional for the lab's one-page + localStorage constraint.
- **Data flow:** Form submission → client-side validation → create report object → save to localStorage → render list and summary counts.

## Run locally
1. Download or clone this repository.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox, or Safari).
3. Add a fictional sample report, search/filter it, change its status, and refresh the page to verify local persistence.

No package installation or build step is required.

## Test checklist
- [ ] Form blocks submission when a required field is missing.
- [ ] A valid report appears with a unique ID and Received status.
- [ ] Search works for ID, category, general location, and summary.
- [ ] Status filter works.
- [ ] Changing status updates the summary cards.
- [ ] Records remain after refreshing the page in the same browser.
- [ ] Delete and clear actions require confirmation.
- [ ] Layout works on desktop and mobile widths.

## Limitations and future improvements
This prototype does not provide user accounts, role-based access, server-side validation, encrypted transmission/storage, audit logs, backups, or multi-user access. A real deployment would require a properly secured backend and database, access policies for authorized barangay personnel, retention and backup procedures, and a privacy review before any real personal data is collected.

## Version
`v0.1.0` — first classroom prototype.
