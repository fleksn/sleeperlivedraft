# Sleeper Draft – Live

A lightweight single‑page web app for monitoring **real‑time draft picks** from [Sleeper](https://sleeper.com) and cross‑referencing them against your **FantasyPros rankings CSV**.

This repo is fully static (HTML + JS + CSS) and can be hosted on **GitHub Pages**.

---

## 🚀 Features
- Connect to any Sleeper draft via Draft ID
- Load rankings via CSV upload, paste, or drag‑drop
- Supports FantasyPros CSV format (auto‑mapped)
- Filters by position & search
- Tier breaks with color coding
- Toggle drafted manually if Sleeper misses a pick
- Recent 20 picks (latest on top, with undo for manual marks)
- Unit tests built‑in for parser & fuzzy name matching

---

## 🛠 Development Notes
- The app is pure HTML/JS/CSS. No build tools required.
- External dependency: [PapaParse](https://www.papaparse.com/) for CSV parsing.
- Uses [Sleeper API](https://docs.sleeper.com/).

---

## 📄 License
MIT — free to use, modify, and share.
