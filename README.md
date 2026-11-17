# Skill Tracker

1. See a visual chart of the development of your skills.
2. Log skill development daily.
3. Decide what skill to work on today.
4. Start projects and goals to improve your skills.

## Features

- **Skills:** on a scale from 0XP (Newcomer) to 10000XP (Master). 1 XP is 1 hour of focused work. There are 10 levels in total.
- **Work on today:** a daily pick based on your last 14 days. It favors skills you haven't touched and weighs how your recent sessions felt: frustration pushes a skill down, a run of exciting sessions keeps your flow going, and a frustrating day boosts skills that have felt good.
- **Pace:** hours per skill over the last 7 days, when each skill will level up at that pace, and a planner for reaching any level by a date.
- **Goals:** checklists of steps, including skill levels that check themselves off. Any step can become its own goal.
- **Projects:** log work against a project and track how close to done it is.
- **Diary:** every entry by day, with mood ratings and level-up markers.
- **Backups:** export everything to a file and restore it on another device.

## Tech

A single-page progressive web app in plain HTML, CSS and JavaScript, with no build step and no framework. Data lives in `localStorage`, a service worker caches the app for offline use, and charts use [Chart.js](https://www.chartjs.org) (MIT, bundled in `vendor/`).

To run it locally, serve the folder with any static server, for example `python3 -m http.server`, then open `http://localhost:8000`.
