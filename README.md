# 🏈 Sleeper Draft Best Available

A simple browser-based app that connects to your live [Sleeper](https://sleeper.app) NFL fantasy draft and shows the **best available players** based on your own rankings.

## ✨ Features

- Load your own rankings via CSV (FantasyPros format supported).
- Auto-updates in real time as picks are made in Sleeper.
- Fuzzy name matching (handles `B. Thomas` ↔ `Brian Thomas Jr.`, `K. Walker` ↔ `Kenneth Walker III`, etc).
- Manual draft checkbox: mark players as drafted if Sleeper’s API doesn’t match them.
- Live sidebar showing the **20 most recent drafted players** (newest at the top).
- Tier breaks with color-coded bands.

## 🚀 How to Use

1. Clone or download this repo.
2. Open `index.html` in your browser (no build step required).
3. Enter your Sleeper **Draft ID**:
   - You can find this in the Sleeper draft URL:  
     `https://sleeper.app/draft/nfl/<DRAFT_ID>`
4. Upload your **rankings CSV** (FantasyPros export or custom CSV with columns: `RK, TIERS, PLAYER NAME, TEAM, POS`).
   - Or click **Load Sample CSV** to test.
5. Click **Start** to begin tracking.
6. Watch as picks come in:
   - Best available players remain listed, grouped by tier.
   - Drafted players (from Sleeper or manual checkboxes) disappear from the list.
   - The right sidebar shows the last 20 drafted players, with newest at the top.

## 🛠 Development Notes

- Built with **plain HTML/JS/CSS**.
- Uses [PapaParse](https://www.papaparse.com/) to parse CSV files.
- Polls Sleeper’s public API every 2 seconds for live updates.
- Manual drafted picks are timestamped so they slot into the drafted list in the correct order.

Feel free to improve!
