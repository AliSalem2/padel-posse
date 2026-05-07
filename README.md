# Padel Posse 🏓

A lightweight, single-file web app for scheduling padel games with your crew — no backend required.

**Live app:** https://alisalem2.github.io/padel-posse/padel-posse.html

---

## Features

- **Shared calendar** — players sign up for time slots that sync in real time across everyone's browser
- **4-player lock-in** — a slot is confirmed once 4 players have joined, with a "Game On!" banner
- **Push notifications** — organisers get an instant phone alert via [ntfy](https://ntfy.sh) when a game fills up
- **No server needed** — data is stored in a free [JSONBin](https://jsonbin.io) bin; the app is a single HTML file
- **Mobile-friendly** — responsive layout optimised for phones

## How it works

1. The organiser creates a free JSONBin account and pastes the API key + Bin ID into the settings panel
2. Share the app link with your group
3. Each player enters their name, picks a time slot, and saves — everyone sees the update live
4. When 4 players lock a slot, the organiser receives a push notification (optional, via ntfy)

## Setup

1. Open the [live app](https://alisalem2.github.io/padel-posse/padel-posse.html)
2. Tap the **Settings** icon
3. Follow the in-app steps to connect your JSONBin bin and (optionally) an ntfy topic
4. Share the URL with your crew — that's it

## Self-hosting

The entire app is a single file (`padel-posse.html`). Drop it anywhere — GitHub Pages, Netlify, a USB stick — and it works.

## Tech stack

- Vanilla HTML / CSS / JavaScript (no build step, no dependencies)
- [JSONBin](https://jsonbin.io) for shared state storage
- [ntfy](https://ntfy.sh) for push notifications
