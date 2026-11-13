Offline Field Issue Tracker

NilePixel Technologies – Cohort 1 Graduation Project

Developed by: [Your Full Name]
Project: Individual Graduation Project
Developer Role: Full-Stack Developer

---

1. Project Introduction

The Offline Field Issue Tracker is a full-stack web application developed by me as my individual graduation project for the NilePixel Technologies Cohort 1 program.

The application is designed to help field workers report infrastructure problems, including broken water points, damaged equipment, service interruptions, safety concerns, and maintenance requirements.

The main purpose of this project is to provide a reliable reporting system that continues working even when internet connectivity is unavailable.

Field workers can create and save reports offline. When an internet connection becomes available, the application automatically synchronizes pending reports with the backend server.

2. Project Objectives

- Build a functional full-stack web application.
- Support offline report creation and storage.
- Synchronize reports automatically when internet connectivity returns.
- Prevent duplicate report submissions.
- Allow coordinators to manage and update reports.
- Maintain an activity history for accountability.
- Provide a responsive interface for Android phones and computers.

3. Technologies Used

Component| Technology
Frontend| HTML, CSS, JavaScript
Backend| Node.js
API| Express.js
Database| SQLite
Offline Storage| IndexedDB
Offline Access| Service Worker
Testing| Node.js test framework

4. Main Features

Dashboard

Displays total reports, pending reports, submitted reports, and resolved reports.

Report Creation

Users can create reports containing:

- Issue category
- Description
- Location
- Priority
- Date and time
- Report status

Offline Functionality

Reports are saved locally using IndexedDB and remain available after refreshing or reopening the application.

Automatic Synchronization

Pending reports are synchronized when internet connectivity returns.

Synchronization states include:

- Pending
- Synchronized
- Failed

Report Management

The application supports the following workflow:

Draft → Submitted → Assigned → In Progress → Resolved

Rejected reports are also supported.

Coordinator Dashboard

Coordinators can view reports, assign issues, and update report statuses.

Activity History

Records report creation, synchronization attempts, errors, and status changes.

5. System Architecture

The application consists of three main layers:

1. Frontend: HTML, CSS, and JavaScript provide the user interface.
2. Backend: Node.js and Express provide the API and business logic.
3. Database: SQLite stores reports and activity records.

IndexedDB provides local storage for offline reports, while the Service Worker supports offline application access.

6. Installation and Setup

Prerequisites

- Node.js
- npm
- A modern web browser

Installation

Clone the repository:

git clone YOUR_GITHUB_REPOSITORY_URL

Open the project directory:

cd offline-field-issue-tracker

Install dependencies:

npm install

Start the application:

npm start

Open the local address configured by the application in your browser.

7. Running Automated Tests

Run:

npm test

The test suite should cover report creation, input validation, status transitions, duplicate prevention, and synchronization behavior.

8. Design Decisions and Assumptions

- Every report receives a unique identifier.
- Locally stored reports must not disappear during synchronization failures.
- Synchronization retries should not create duplicate server records.
- Invalid status transitions must be rejected.
- Report history should preserve important events.
- Failed synchronization should be visible to the user.
- Submitted reports should retain their history.

9. Testing Priorities

The main testing priorities are:

- Report creation and validation.
- Offline data persistence.
- Synchronization and retry handling.
- Duplicate report prevention.
- Valid and invalid status transitions.
- Activity history recording.
- Responsive interface behavior.

10. Known Limitations

Document any incomplete functionality, browser compatibility issues, or deployment limitations identified during testing.

11. AI and Development Tool Disclosure

AI-assisted development tools, including ChatGPT and Replit AI, were used for development guidance, debugging assistance, code suggestions, and documentation preparation.

I reviewed and evaluated the suggestions used in the project and remain responsible for understanding, testing, and explaining the final implementation.

12. Developer Reflection

Approximate development time: [Enter actual hours spent]

What I learned:

- Full-stack application development.
- Frontend and backend integration.
- Database management.
- Offline-first application design.
- Data synchronization.
- Testing and debugging.

Future Improvements:

- Add authentication and role-based access.
- Improve synchronization conflict handling.
- Add report image attachments.
- Improve automated test coverage.
- Deploy the application for real-world use.

---

13. Developer Declaration

I developed this Offline Field Issue Tracker as my individual graduation project for NilePixel Technologies Cohort 1.

This project represents my practical application of the concepts and skills learned during the three-day bootcamp.

Developer: [maryamawit yohannes]

Project: Offline Field Issue Tracker

Program: NilePixel Technologies – Cohort 1# issue-offline-tracking-app-