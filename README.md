# HabitTerra 🌱

A responsive habit tracker with a virtual garden, rewards, and local persistence. Built with React and Vite.

## Features

- Add, edit, complete, and delete daily habits
- Earn water drops, seeds, and growth points for completing habits
- Plant virtual plants using seeds
- Daily progress and a weekly progress overview
- LocalStorage persistence (no account required)
- Export your data as JSON and reset local data
- Responsive desktop sidebar and mobile bottom navigation

## Requirements

- Node.js 18 or newer
- npm

## Run locally

```bash
npm install
npm run dev
```

Vite prints a local URL (usually `http://localhost:5173`). Open it in your browser.

## Build for production

```bash
npm run build
npm run preview
```

## Project layout

```text
HabitTerra/
├── public/
├── src/
│   ├── components/       # Reusable UI components
│   ├── pages/            # Overview, habits, garden, progress, settings
│   ├── utils/            # Local storage and reward helpers
│   ├── App.jsx           # App state, actions, and page routing
│   ├── main.jsx          # React entry point
│   └── index.css         # Responsive visual design
├── index.html
├── package.json
└── vite.config.js
```

## Notes

- Data is stored in the current browser on the current device. Clearing browser site data removes it, so export backups periodically.
- The weekly bars are a visual placeholder in this MVP; historical analytics can be implemented next.
- The starter state is demo data. Use Settings → Reset data to return to the starter state.
- Rewards are applied once per habit per day. Unchecking a habit reverses that habit's rewards.
