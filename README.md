UPSC CSE Preparation Tracker

A single-page tracker for UPSC Civil Services Examination preparation. It is one HTML file (index.html) built with plain HTML, CSS and JavaScript. There is no backend, no login and no paid API.

All your data is saved in your browser's localStorage.

Features
Embedded syllabus: Prelims GS Paper I and CSAT, Mains Essay, GS I, GS II, GS III and GS IV, organised as Paper → Subject → Topic → Subtopic.
Per-subtopic tracking: Notes, Learning and Revision checkboxes, a status badge (a subtopic is Completed only when all three are ticked), a personal notes field, a confidence level, a PYQ tag, a last-revised date and a study timer with manual time entry and session history.
Time roll-up: time is totalled for each topic, subject, paper and stage, and overall.
Dashboard: progress percentages, study time (today, this week, total), streak, countdown to the exam date (default 25 May 2028), revisions due and a daily-target bar.
Revision planner: spaced repetition at 3, 7, 15, 30 and 60 days, with overdue items flagged.
Syllabus Memory: flashcards, blank recall, topic recall, paper structure, a 50-question quiz and an expandable syllabus map.
Pomodoro timer: configurable focus and break lengths, with focus time added to a chosen subtopic.
Logs: mock tests, answer writing and current affairs.
Analytics: completion, time per paper, subject and topic, a weekly study chart and more.
Search and filters: global search plus filter chips on the Prelims and Mains pages.
Settings: dark mode, exam date, daily and weekly targets, Pomodoro durations, optional subject, JSON export and import, reset.
Run locally

Download index.html and open it in any modern browser. Nothing needs to be installed.

Deploy on GitHub Pages
Create a public repository.
Upload index.html to the root of the repository.
Go to Settings → Pages, choose Deploy from a branch, select main and / (root), then save.
Open https://<your-username>.github.io/<repository-name>/ after a minute or two.
Your data
Progress is stored per browser and per web address. A different browser, device or address starts empty.
Use Settings → Export JSON regularly as a backup, and Import JSON to restore it or move to another device.
Clearing your browser data erases your progress.
Updating the syllabus

The syllabus is a JavaScript constant named UPSC_SYLLABUS inside index.html. Each subject uses this format:

js
sb("Subject name",
  tp("Topic name", ["Subtopic 1", "Subtopic 2"])
)

Progress is saved under the paper, subject and topic names. Renaming an item will detach its saved progress, so add new items rather than renaming existing ones.

Known limitations
Offline use relies on your browser keeping the page cached after the first load. There is no service worker yet.
The Optional subject is a flat list of items you add yourself, not a nested syllabus.
The Revision Planner has no paper, subject or topic filter.
Mock-test analysis is broken down by paper, not by subject.
The layout is designed to adapt to desktop, tablet and phone screens, but it has not been tested on real devices.
