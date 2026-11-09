# StudyTracker

A simple **student task planner** mobile app built with **React Native (Expo)**. Add tasks with a subject, deadline and priority, tick them off when done, and review them in a Completed list. Data is saved on the device, so it works offline.

## Features

- **Add tasks** with a title, subject, priority (High / Medium / Low), deadline and notes
- **Smart deadline sorting**: tasks are sorted by nearest deadline; the deadline can be typed in common formats (`Dec 5`, `12/5`, `2026-12-05`) or picked from a calendar
- **Search** tasks by title or subject
- **Complete** tasks with a checkbox and review them in the **Completed** tab
- **Edit and delete** tasks, with a confirmation before deleting
- **Form validation**: title, priority and deadline are required, with clear error messages
- **Offline storage**: tasks are stored on the device with AsyncStorage
- Works on **Android, iOS and web**

## Tech Stack

| Area | Technology |
|------|------------|
| Framework | React Native 0.86, Expo SDK 57 |
| Navigation | Expo Router (file-based routing, bottom tabs) |
| State | React Context |
| Storage | AsyncStorage |
| Language | JavaScript |
| Icons | react-native-svg |

## Getting Started

Requires **Node.js 22**.

```bash
git clone https://github.com/eltlhibn/StudentPlanner.git
cd StudentPlanner
npm install
npm start
```

Then scan the QR code with the **Expo Go** app (Android / iOS), or press `w` to open it in the browser.

| Command | What it does |
|---------|--------------|
| `npm start` | Start the Expo dev server |
| `npm run android` / `npm run ios` | Open on an emulator or device |
| `npm run web` | Run in the browser |

## Project Structure

```
src/
├── app/            # Screens and routes (Expo Router)
│   ├── (tabs)/     # Tasks, Add Task, Completed
│   ├── task/       # Task details
│   └── edit-task/  # Edit task
├── components/     # Reusable UI (TaskCard, TaskForm, ...)
├── constants/      # Theme colours
├── state/          # App state and storage (AppContext)
└── utils/          # Deadline parsing, helpers
```

## Author

**Ella Talahiban**: [github.com/eltlhibn](https://github.com/eltlhibn)
