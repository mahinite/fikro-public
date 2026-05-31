<div align="center">

# Fikro

**Capture ideas fast. Retrieve them when it matters.**

A lightweight, offline-first idea manager for creators, writers, and builders.

![Version](https://img.shields.io/badge/Version-1.2-FACC15?style=for-the-badge&labelColor=15181F)
![Platform](https://img.shields.io/badge/Platform-Windows-FACC15?style=for-the-badge&labelColor=15181F)
![Status](https://img.shields.io/badge/Status-Beta-FACC15?style=for-the-badge&labelColor=15181F)
![License](https://img.shields.io/badge/License-MIT-FACC15?style=for-the-badge&labelColor=15181F)

</div>

---

## What is Fikro?

Fikro is a desktop tool that helps you capture, organise, and retrieve creative ideas — without friction.

Every idea starts with a **hook**: a short, punchy line that captures the core angle before the thought disappears. You attach a pattern, a topic, a note, a reference link — and it's stored locally, permanently, and instantly searchable.

When you're stuck, Fikro picks one for you.

No accounts. No syncing. No internet required.

---

## The Problem

Creators lose ideas constantly. A thought in the shower. A thread you meant to write. A video angle you kept meaning to develop. It ends up in a Notes app, a voice memo, a forgotten Notion page, or nowhere at all.

The issue isn't lack of ideas — it's that there's no reliable place to put them, and no easy way to get them back when you actually need to create.

Fikro is that place.

---

## Features

- **Hook-first capture** — every idea begins with a short, memorable line (max 120 chars) that forces clarity before context
- **Pattern tagging** — categorise ideas by type (Reflection, Tutorial, Story, Wake-Up, etc.) with custom colours; create, rename, and reorder patterns to fit your workflow
- **Topic labels** — add freeform topic tags like "AI", "Health", or "Finance" for cross-pattern filtering
- **Notes and reference links** — attach extended context and source URLs to any idea
- **Random idea picker** — "Give Me Idea" pulls a random active idea from your pool when you don't know what to create next
- **Recent picks history** — the last 10 randomly picked ideas are tracked in the sidebar for quick access
- **Multiple workspaces** — separate independent vaults for different projects, clients, or creative modes
- **Status pipeline** — move ideas from active → archived → bin; bulk-archive or bulk-delete when you need to clean up
- **Two view modes** — Cards (grid) for browsing, Feed (list) for scanning large libraries fast
- **Real-time search and sort** — filter by pattern, search by keyword, sort by date or category
- **Global hotkey** (`Ctrl+Shift+Space`) — open the quick-add modal from anywhere on Windows without switching windows
- **System tray** — Fikro stays running in the background; double-click the tray icon to bring it back
- **Local HTTP API** — a background server on port `13457` lets external tools and browser extensions push ideas directly into Fikro
- **Fully offline** — all data is stored as plain JSON in `%APPDATA%\Fikro`; no cloud, no account, no tracking

---

## How It Works

**1. Capture**
Press `Ctrl+Shift+Space` from anywhere. Type your hook. Assign a pattern. Save with `Enter`. Done in under ten seconds.

**2. Organise**
Ideas land in your active Workspace. Move them to Archive once used. Bin them when they're no longer relevant. Filter and search at any time.

**3. Retrieve**
Open Fikro when you're ready to create. Filter by pattern or topic, or hit **Give Me Idea** to let Fikro pick something from your active pool at random.

**4. Create**
Mark the idea as Used when you act on it. It moves to Archive automatically, keeping your active list clean and relevant.

---

## Why It Exists

Most idea tools are built for project management, not for the creative moment before a project starts. They're too heavy, too connected, and too slow to open when a thought hits.

Fikro is built for the gap between having an idea and acting on one — a place that's always open, always fast, and never gets in the way.

---

## Tech Stack

- **Python 3.11** — application logic and data layer
- **PySide6** — native window, system tray, and global hotkey registration
- **QWebEngineView + QWebChannel** — the UI is a self-contained HTML/CSS/JS frontend embedded in the app
- **Python `http.server`** — lightweight background API for external integrations
- **PyInstaller** — packaging into a standalone Windows executable
- **Plain JSON** — no database; all data is human-readable and portable

---

## Status

Fikro is in active development. Core functionality is stable and used daily.

Upcoming:
- Import / Export (JSON backup and restore)
- Chrome Extension (save ideas directly from the browser)
- macOS support

---

## Get Involved

- **Star this repo** to follow progress
- **Open an issue** to report a bug or suggest a feature
- **Fork and build** — contributions are welcome

---

<div align="center">

Built by **[Mahinite](https://github.com/mahinite)** &nbsp;·&nbsp; MIT License

</div>
