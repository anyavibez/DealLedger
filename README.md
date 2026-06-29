# lovely money ♥

A private, love-themed shared money tracker for **advik33** and **anyacutie1** — now with **cross-device sync** via Firebase Realtime Database.

Track income, expenses, and payments together. Changes made on one device appear instantly on the other. No server to run, just deploy to GitHub Pages and go.

---

## Features

- **Add Money** — log income with a note
- **Cut Expenses** — track every spend
- **Pay Someone** — record payments to anyone
- **Cross-Device Sync** — changes sync instantly via Firebase
- **Persistent Login** — stay logged in until you press Sign Out
- **Balance Overview** — see total + recent change
- **Stats Panel** — earned, spent, transaction count
- **Activity Log** — full searchable history with filters
- **Export Backup** — download your data as JSON
- **Keyboard Shortcuts** — press `1` / `2` / `3` for quick actions
- **Dark Love Theme** — floating hearts, rose gradients, glassmorphism
- **Real-Time Updates** — Firebase listener keeps all devices in sync

---

## Login Credentials

| User     | Password     |
|----------|-------------|
| `advik33` | `advik@33` |
| `anyacutie1` | `anya@cutie1` |

---

## How to Use (Development)

1. Open `index.html` in any browser (or deploy to GitHub Pages)
2. Sign in with your credentials
3. Use **+ Add / - Cut / → Pay** to log transactions
4. Switch between **Overview** and **Logs** tabs
5. Search, filter, or export your logs anytime

### Cross-Device Sync Setup

The app uses **Firebase Realtime Database** for cross-device sync. To use it:

1. Go to https://console.firebase.google.com and create a project
2. Enable **Realtime Database** (start in test mode)
3. Register a **Web app** and copy the Firebase config
4. Open `index.html`, find the `firebaseConfig` object (around line 860), and paste your config
5. Deploy to GitHub Pages or any static host

No backend server needed. The Firebase SDK talks directly to the cloud.

---

## File Structure

```
lovely-money/
  index.html       — single-file app (landing page + dashboard + all logic)
  README.md        — this file
```

Single HTML file. No build tools, no frameworks, no server.

---

## Data Privacy

Data is stored in **Firebase Realtime Database** (cloud) so both users can access it from any device. For local caching, the app also keeps a copy in memory during the session. Use the **Export** button to download a JSON backup anytime.

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- **Firebase Realtime Database** (cross-device sync)
- **BroadcastChannel API** (same-browser multi-tab sync)
- Google Fonts (Inter + Fraunces)
- CSS custom properties, backdrop-filter glassmorphism

---

Made with infinite love ♥ for advik33 & anyacutie1.
