# Affirmation Studio

A premium single-page affirmations app built with plain HTML, CSS, and JavaScript — no dependencies, no build step.

## Features

### Core Experience
- **Daily seeded affirmation** — the same calm anchor every morning, changing each new day
- **Auto-rotation** — a fresh affirmation every 10 seconds with a visual progress bar
- **Animated transitions** — smooth fade between affirmations
- **Category filtering** — All moods · Self-worth · Love · Calm · Gratitude · Growth
- **Reflection prompt** — a thoughtful question tailored to each affirmation's category
- **500+ affirmations** — curated core set plus a generative library for variety

### Personalization
- **🌙 Dark mode** — toggle between warm light and deep dark themes; persists across sessions
- **🔥 Streak counter** — tracks consecutive daily visits to build a mindful habit
- **☀️ Time-of-day greeting** — morning, afternoon, evening and night messages
- **⚓ Daily anchor** — today's seeded affirmation shown as a persistent reference

### Saving & History
- **♡ Favorites** — save up to 40 affirmations; click any saved one to reload it
- **◷ Recent history** — last 12 affirmations, clickable to revisit
- **Remove individual favorites** — hover to reveal the remove button
- **Clear all** buttons for both favorites and history

### Journaling
- **✎ Reflection Journal** — write thoughts tied to a specific affirmation
- Saves up to 25 entries with timestamps and category labels
- Character counter (600 char limit)
- Entries displayed in a scrollable feed below the input

### Wellness Tools
- **◎ Breathing Guide** — guided 4·7·8 technique (Inhale 4s · Hold 7s · Exhale 8s)
- 4 complete cycles with live countdown and animated ring
- Calming colour transitions during each breath phase

### Sharing & Export
- **📤 Share button** — uses Web Share API on mobile; falls back to clipboard copy
- **⎘ Copy** — copies the current affirmation instantly
- **🖨 Print favorites** — opens a clean print-ready list of all saved favorites

### Feedback
- **Animated toast notifications** — unobtrusive confirmations for every action
- **Confetti burst** — celebratory animation when saving a new favorite
- **Animated stat counters** — numbers count up smoothly in the Overview panel

### Accessibility & Input
- **Keyboard shortcuts**
  - `Space` — new affirmation
  - `F` — toggle favorite
  - `C` — copy to clipboard
- **Swipe left / right** — next affirmation on touch devices
- `aria-live` regions for screen readers
- `aria-pressed` on category chips

### Data Persistence
- Everything stored in `localStorage` — no account, no server required
- Storage keys versioned (`v3`) to avoid conflicts with older saved data

---

## Run

Open `index.html` directly in any modern browser, **or** start the local dev server:

```bash
npm run dev
```

Then visit **http://localhost:3000**

---

## Project Structure

```
AFFIRMATIONS--main/
├── index.html      # Entire app — HTML + embedded CSS + JS
├── server.js       # Minimal Node.js static file server
├── package.json    # npm scripts
└── README.md
```

---

## Tech Stack

| Concern | Choice |
|---------|--------|
| Structure | Semantic HTML5 |
| Styling | Vanilla CSS with custom properties (design tokens) |
| Logic | Vanilla JavaScript (ES2020+) |
| Fonts | Google Fonts — Playfair Display + Inter |
| Storage | localStorage |
| Server | Node.js `http` module (dev only) |

No frameworks. No build tools. No dependencies.
