# Skill Tracker

A daily log of the time you put into your skills, turned into levels. Log the hours you put into any skill you choose and watch each one level up from Newcomer to Master.

**Private by design:** there's no account and no server. Everything is saved on your own device and works offline. Install it on your phone from the browser like an app.

## Features

- **XP and levels:** 1 focused hour of making = 1 XP, across 10 levels from Newcomer (0 XP) to Master (10,000 XP). Narrower crafts can earn more XP per hour.
- **Rust:** a skill left untouched for over a year slowly loses effective level, capped at 30%. Lifetime XP never disappears.
- **Work on today:** a daily pick based on your last 14 days. It favors skills you haven't touched and weighs how your recent sessions felt: frustration pushes a skill down, a run of exciting sessions keeps your flow going, and a frustrating day boosts skills that have felt good.
- **Pace:** hours per skill over the last 7 days, when each skill will level up at that pace, and a planner for reaching any level by a date.
- **Goals:** checklists of steps, including skill levels that check themselves off. Any step can become its own goal.
- **Projects:** log work against a project and track how close to done it is.
- **Diary:** every entry by day, with mood ratings and level-up markers.
- **Backups:** export everything to a file and restore it on another device.

## Tech

A single-page progressive web app in plain HTML, CSS and JavaScript, with no build step and no framework. Data lives in `localStorage`, a service worker caches the app for offline use, and charts use [Chart.js](https://www.chartjs.org) (MIT, bundled in `vendor/`).

To run it locally, serve the folder with any static server, for example `python3 -m http.server`, then open `http://localhost:8000`.
