# gym-log-dashboard
Minimalist yearly gym tracker — click any day to log it, click again to unlog. Saves to browser storage, auto-unlocks future days as they arrive. No server, no login, no dependencies.

<img width="600" alt="image" src="https://github.com/user-attachments/assets/b0c20fbe-0c14-4167-b134-72e81c1119e2" />

## Live site

[saamiyalaroia.github.io/gym-log-dashboard](https://saamiyalaroia.github.io/gym-log-dashboard)

## Features

- Click any day cell to toggle it as a gym day
- Future days are locked and unlock automatically as the date arrives
- Today is highlighted with a green border
- Stats update live: total sessions, this month, this week, best month, current streak
- Mini frequency bar next to each month shows your consistency at a glance
- All data saved to browser localStorage — no account needed

## Usage

Open the site and click any past or present day to log it. Click again to unlog. That's it.

To log a missed day, just click it retroactively — the calendar goes back to January 1st.

## Deployment

This is a single static `index.html` file with no build step or dependencies.

**GitHub Pages:**
1. Upload `index.html` to any GitHub repository
2. Go to Settings → Pages → Deploy from branch → main → Save
3. Your site is live at `https://saamiyalaroia.github.io/gym-log-dashboard`

**Local:**
Just double-click `index.html` — it opens directly in your browser.

## Data

Gym days are stored in your browser's `localStorage` under the key `gym2026`. Data persists as long as you use the same browser. It is not synced across devices.

To back up your data, open the browser console and run:
```js
console.log(localStorage.getItem("gym2026"));
```
Copy the output somewhere safe.
