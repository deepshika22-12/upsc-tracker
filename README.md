# 🎯 UPSC CSE Preparation Tracker

A free, interactive tracker for UPSC Civil Services Examination preparation. Track every subtopic, log your study time, plan revisions and test yourself on the syllabus, all in one page.

### 🔗 [Open the live app](https://deepshika22-12.github.io/upsc-tracker/)

Built with plain HTML, CSS and JavaScript. There is no backend, no login and no paid API. Everything is saved in your own browser.

---

## ✨ Features

### 📚 Complete syllabus tracking
- Prelims GS Paper I and CSAT
- Mains Essay, GS Paper I, GS Paper II, GS Paper III and GS Paper IV
- Organised as **Paper → Subject → Topic → Subtopic**
- Optional subject Paper I and Paper II, where you add your own items

### ✅ For every subtopic
- 📖 Notes, 🧠 Learning and 🔁 Revision checkboxes
- Status badge: Not started, In progress or Completed (all three ticked)
- Personal notes field
- Confidence level: Low, Medium or High
- PYQ tag: Prelims PYQ, Mains PYQ, Both or Not asked
- Last revised date
- Start/Stop study timer, manual time entry and session history

### ⏱ Time tracking
- Time rolls up automatically to topic, subject, paper and stage, and to your overall total
- Pomodoro timer with adjustable focus and break lengths
- Focus time is added to the subtopic you pick

### 📊 Dashboard and analytics
- Overall, Prelims and Mains progress
- Today's, this week's and total study time
- Study streak and countdown to your exam date
- Weakest and strongest subjects
- Weekly study chart, time per paper, subject and topic

### 🔁 Revision planner
- Spaced repetition at 3, 7, 15, 30 and 60 days
- Overdue revisions are flagged

### 🧠 Syllabus Memory
- Flashcards, blank recall and topic recall
- Paper structure and an expandable syllabus map
- A 50-question quiz with instant feedback and a best score

### 📝 Logs
- Mock tests, answer writing and current affairs

### 🔍 Search, filters and settings
- Global search across papers, subjects, topics, subtopics and your notes
- Filter chips such as Incomplete, Fully completed, Pending revision, Low confidence and PYQ
- Dark mode, exam date, daily and weekly study targets
- Export and import your data as JSON, and a reset button

---

## 🚀 Run it yourself

**Locally:** download `index.html` and open it in any modern browser.

**On GitHub Pages:**
1. Create a public repository and upload `index.html` to its root.
2. Go to **Settings → Pages**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
3. Your site appears at `https://<your-username>.github.io/<repository-name>/`.

---

## 💾 Your data

- Progress is saved in your browser's `localStorage`, separately for each browser, device and web address.
- Use **Settings → Export JSON** regularly as a backup, and **Import JSON** to restore it or move to another device.
- Clearing your browser data erases your progress.

---

## 🛠 Updating the syllabus

The syllabus is a JavaScript constant named `UPSC_SYLLABUS` inside `index.html`. Each subject is written like this:

```js
sb("Subject name",
  tp("Topic name", ["Subtopic 1", "Subtopic 2"])
)
```

Progress is saved under the paper, subject and topic names. Renaming an existing item detaches its saved progress, so add new items instead of renaming old ones.

---

## ⚠️ Known limitations

- Offline use relies on your browser keeping the page cached after the first load. There is no service worker yet.
- The Optional subject is a flat list you fill in yourself, not a built-in syllabus.
- The Revision Planner has no paper, subject or topic filter.
- Mock-test analysis is broken down by paper, not by subject.
- The layout adapts to desktop, tablet and phone screens, but it has not been tested on real devices.

---

## 🤝 Contributing

Found a bug or a syllabus error? Open an issue or submit a pull request.

---

Made for UPSC aspirants. Good luck with your preparation! 🇮🇳
