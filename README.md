# Social Engineering Detective

A self-contained, offline-capable browser game for **GCSE Computer Science (AQA 8525)** students revising **3.6.2.1 Social Engineering**.

Students act as a cyber security investigator: each case asks them to identify the **attack type**, the **information being targeted**, and the **best protection method**, with instant feedback and scoring.

## Learning Objectives (AQA 8525 • 3.6.2.1)
- Define social engineering
- Understand that social engineering is the manipulation of people to obtain confidential information
- Identify and explain:
  - Phishing
  - Blagging (Pretexting)
  - Shoulder Surfing (Shouldering)
- Describe how each attack can be prevented

## What’s Included
- Fully offline single-file web app: [social-engineering-detective.html](./social-engineering-detective.html)
- Scenario bank (randomised each playthrough, no repeats):
  - 8 phishing scenarios
  - 8 blagging/pretexting scenarios
  - 8 shoulder surfing scenarios
  - 8 decoy scenarios (not social engineering)
- Game flow:
  - Welcome screen
  - Learning screen (definitions + prevention)
  - Randomised game scenarios with immediate feedback
  - End screen with final score, percentage, performance rating, and review of incorrect answers
- Bonus mode:
  - “Spot the Clues” phishing email mockup built with HTML/CSS (no images)
  - Click suspicious elements to earn bonus points
- Teacher Dashboard:
  - Hidden button labelled “Teacher Dashboard”
  - Shows question counts, categories covered, AQA mapping, learning objectives

## How to Run Locally (No Install)
1. Download or clone this repository.
2. Open `social-engineering-detective.html` in a browser (Chrome, Edge, Firefox, Safari).
3. Use:
   - Learning Screen to revise key definitions
   - Start Game to begin the main investigation
   - Bonus: Spot the Clues for additional practice

## GitHub Pages
This repository is configured to deploy automatically to GitHub Pages on every push to `main` using a GitHub Actions workflow:
- Workflow file: [.github/workflows/deploy.yml](./.github/workflows/deploy.yml)
- Static deployment behaviour:
  - If no build output folder exists, the workflow copies `social-engineering-detective.html` to `site/index.html` and publishes `site/`

## Classroom Notes
- The app runs entirely in the browser and does not require an internet connection once downloaded.
- Sound effects are generated using browser audio APIs (no external assets).
- The “Not Social Engineering” decoy questions help students avoid over-labelling everything as phishing.

## File Overview
- `social-engineering-detective.html` — complete app (HTML + CSS + JavaScript in one file)
- `.github/workflows/deploy.yml` — GitHub Pages deployment workflow
