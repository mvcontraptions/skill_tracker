# Skill Tracker

What you can do:
1. See a visual chart of the development of your skills.
2. Log skill development daily.
3. Decide what skill to work on today.
4. Start projects and goals to improve your skills.
5. Measure your pace and predict when you will level up next!

## Features

- **Skills:** on a scale from 0XP (Newcomer) to 10000XP (Master). 1 XP is 1 hour of focused work. There are 10 levels in total.
- **Daily recommendation:** a daily pick based on your last 14 days. It favors skills you haven't touched and weighs how your recent sessions felt.
- **Pace:** the hours you spent on a skill over the last 7 days. It also calculates when each skill will level up at that pace.
- **Goals:** checklists of steps, including skill levels that check themselves off. Any step can become its own goal.
- **Projects:** log work against a project and track how close to done it is.
- **Diary:** every entry by day, with mood ratings and level-up markers.
- **Backups:** export everything to a file and restore it on another device.

## Tech

A single-page progressive web app in plain HTML, CSS and JavaScript, with no build step and no framework. Data lives in `localStorage`, a service worker caches the app for offline use, and charts use [Chart.js](https://www.chartjs.org) (MIT, bundled in `vendor/`).

To run it locally, serve the folder with any static server, for example `python3 -m http.server`, then open `http://localhost:8000`.

Vibe coded with Claude Opus.
