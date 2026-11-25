# Lab 1 Submission Guide

Use this as a draft when filling in the activity form. Replace **[Barangay Name]** with your actual community name before submitting.

## 1. Pick the problem

- **App name:** Barangay Peace & Order — Incident Blotter Tracker
- **Your community:** [Barangay Name], [Municipality/City], Philippines
- **Who has this problem?:** Barangay peace-and-order desk staff who receive and follow up on community concerns; residents who report concerns are the people served.
- **How do they handle it today?:** Reports may be received verbally, through calls, or in handwritten notes and separate records. This can make it harder to find a report and check its follow-up status.
- **Why is it small enough for one page + localStorage?:** The lab prototype focuses on one workflow only: add a sample report, view/search/filter the list, and update its status. It uses fictional data stored in one browser and does not need a backend for the demonstration.
- **Data note:** Use synthetic/fictitious reports only. Do not store real personal or incident information in this prototype.

## 2. Write the FR-01

- **As a:** Barangay peace-and-order desk staff member
- **I can:** record an incident report and update its follow-up status
- **So that:** community concerns can be organized and their progress can be checked

### Acceptance criteria
1. When I submit a report with a date, category, general location, and short summary, the app creates a unique report ID and displays it with the status **Received**.
2. When I search by report ID, category, location, or summary, or choose a status filter, the app displays only matching reports.
3. When I update a report to **Under Review** or **Resolved**, the new status and summary counts are saved and remain after I refresh the page.

## 3. Build with the demo steps

Use the instructor's exact demo-step names if they are shown in your class materials. For your project, you can demonstrate the workflow in this order:
1. Open the one-page app.
2. Explain the classroom-only privacy warning.
3. Point out the three status summary cards.
4. Show the incident report form.
5. Submit a fictional report with all required fields.
6. Show the generated report ID.
7. Find the report using the search box.
8. Filter the list by Received.
9. Change the report status to Under Review.
10. Show the count and status update.
11. Change the report status to Resolved.
12. Refresh the browser and show that localStorage kept the record.
13. Delete a demo report or reload the sample records.
14. Resize to a mobile-width screen and show the responsive layout.

## 4. GitHub checklist

- Create a **public** GitHub repository named `barangay-peace-order-blotter` (or a similar available name).
- Upload the files in this folder.
- Make at least six small commits; do not make one giant commit. Suggested commit sequence:
  1. `chore: add project structure and lab documentation`
  2. `feat: build responsive one-page layout`
  3. `feat: add incident report form and validation`
  4. `feat: save demo reports in localStorage`
  5. `feat: add search and status filters`
  6. `feat: add report status updates and delete actions`
  7. `docs: add test checklist and v0.1.0 notes`
- Create a branch named `feature/blotter-tracker`, make at least one meaningful change there, open a pull request, and merge it into `main`. A pull request must actually be created and merged on GitHub to count.
- Create a GitHub Release tagged **`v0.1.0`** with release title **`v0.1.0 — First Blotter Tracker Prototype`**.
- Copy the public repository URL for the activity form.

## 5. README and project brief

The folder already includes `README.md` and `PROJECT_BRIEF.md`. Read them and update the community name and any details that are specific to your barangay. Keep the FR-01 wording consistent between the form, README, and project brief.

## 6. Prompt log

`PROMPT_LOG.md` has the first AI-use entry for this request. Add one entry per additional prompt you use. Do not claim that you wrote code without AI assistance if you used AI-generated help; describe what you reviewed and changed yourself.

## 7. Video demo (2–3 minutes)

Suggested recording outline:
- **0:00–0:20:** State the barangay problem and the app's goal.
- **0:20–0:45:** Explain the FR-01 user story and the three statuses.
- **0:45–1:40:** Add a fictional report, search it, filter it, and update its status.
- **1:40–2:10:** Refresh to demonstrate localStorage persistence and show the mobile layout.
- **2:10–2:30:** State the limitations: sample data only, no login, no backend, not for official records.

Upload the recording as an unlisted video if allowed by your instructor, then paste the share link in the activity form.

## Links to paste into the activity form
- **Public GitHub repo:** [paste your actual public repository URL]
- **Video demo:** [paste your actual video URL]
