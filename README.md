# Assignment 4 — Forms and Validation

**Project concept:** Railway ticket booking, hackathon registration, and a café reservation form.

This project uses HTML, Bootstrap 5, and custom CSS. It intentionally uses **no JavaScript** and no `novalidate` attribute, following the assignment instructions.

## Files

- `index.html` — Task 1: responsive railway booking form.
- `styles.css` — shared visual design and Task 1 custom styling.
- `task2.html` — Task 2: AITU Hack 2026 registration with native HTML validation.
- `task3.html` — Task 3: rebuilt café reservation form with labels, semantic structure, and responsive Bootstrap layout.
- `report-template.md` — report structure and places to add your screenshots, name, group, results, and GitHub URL.

## Run locally

1. Download and extract the project folder.
2. Open `index.html` in Chrome, Firefox, or Edge.
3. Open `task2.html` and `task3.html` separately to inspect Tasks 2 and 3.
4. Internet is needed for the Bootstrap CDN and Google Font. The HTML forms still exist offline, but styling may be reduced.

## Responsive checks

Use browser developer tools and test the Task 1 page at:
- 375px wide (phone)
- 1280px wide (laptop)

The layout uses Bootstrap's grid and responsive utility classes rather than fixed widths or absolute positioning.

## Task 2 validation examples to test

| Field | Valid example | Invalid example |
|---|---|---|
| Full name | `Anna-Maria Lee` | `A` |
| University email | `a.fedenko@astanait.edu.kz` | `a.fedenko` |
| Age | `18` | `15`, `31`, `18.5` |
| Team size | `4` | `5`, `2.5` |
| Track | `Web` | `Choose…` |
| Arrival day | `21.11.2026` | `25.11.2026` |
| Check-in | `10:30` | `10:15`, `19:00` |
| Entry fee | `1500` | `1250`, `6000` |
| Experience | `Beginner` | no selection |
| GitHub profile | empty or `https://github.com/yerassyl-dev` | `github.com/yerassyl-dev` |
| Password | `Astana2026` | `short` |
| Motivation | 50–300 characters | 49 characters |
| Rules agreement | checked | unchecked |

**Important:** HTML's built-in email validation checks email format, not whether an address belongs to the university domain. HTML `type="url"` validates URL syntax, but a browser's exact error wording can vary. The `:user-invalid` and `:user-valid` pseudo-classes depend on browser support and interaction state.

## Before submission

- Replace the placeholders in the report with your actual name and group.
- Add your own screenshots: Task 1 at 375px and 1280px, Task 2 validation examples, and Task 3.
- Complete Task 2's result table using tests you personally run in your browser.
- Complete Task 3's issue table after comparing your corrected form to the original bad form shown in the assignment PDF. That original code is not included in this project folder, so the report template provides suggested usability issues to verify.
- Write the conclusion in your own words.
- Upload the source files and your completed report to your own GitHub repository, then put the real repository URL in the report.
- Read the code and practice explaining each field, attribute, and CSS rule before your defense.

The forms use `action="#"` for demonstration. They validate in the browser but do not save or send registrations or bookings to a server.
