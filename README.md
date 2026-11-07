# Vihanga LMS

Local-first instructor dashboard for the **Complete MERN Stack Web Development Programme**.

## Run it

Open `index.html` directly in a modern browser, or serve this folder with any static server:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

No backend, build step, authentication, or package installation is required. Progress is stored locally in namespaced keys beginning with `vihanga-lms:v1:`.

## What is included

- Five phases, 26 teaching weeks, and exactly 52 detailed sessions.
- Roadmap modules with expandable instructor notes and module checks.
- Weekly Plan with two 120-minute sessions per week, time allocations, homework, resources, and session completion.
- Project Board with 26 weekly assignments, five phase projects, and the Task & Project Management Platform capstone.
- Local project status, URLs, notes, feedback, and score fields with URL/score validation.
- Resource library with three shared resources per session: official documentation, a video search link deliberately marked for instructor verification, and a longer-form book reference.
- Local reset confirmation and refresh-safe navigation/progress.

## Resource verification policy

Official documentation and legitimate publisher/author links are included directly. Video entries use accurate YouTube search URLs instead of fabricated video IDs or durations; they are labelled `verify before use` so the instructor can select a current lesson before class.

## Data architecture

The curriculum is represented in `app.js` as `phases`, `moduleData`, `weekSpecs`, `sessions`, `resources`, `weeklyAssignments`, `phaseProjects`, and `capstone`. Session and project records use stable identifiers such as `W01-S01`, `WA-01`, `PA-BE-01`, and `CAP-01`.
