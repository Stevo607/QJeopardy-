# README: Quality Jeopardy - Enhanced Edition (Host Intervention)

## Overview

**Quality Jeopardy - Enhanced Edition** is a browser-based, interactive training game modeled after the classic Jeopardy format. It is designed to enhance food safety and quality knowledge in a collaborative, engaging environment for teams. This tool is especially relevant for plant teams, quality professionals, and anyone supporting a robust food safety culture.

This edition features advanced host controls, real-time score tracking, final jeopardy, and a dynamic, mobile-friendly interface. Game questions span food safety, GMPs, FSMA, allergens, HACCP, and chocolate production—aligning with food manufacturing best practices.

---

## Features

* **Category-based Jeopardy gameplay:** 6 categories, 5 questions per category (30 total)
* **Multiple player support:** Add up to 8 players; real-time score display and progression
* **Host intervention:** Host can select which player answers, rotate control, and judge responses
* **Daily Double:** Randomly selected questions allow wagering
* **Final Jeopardy round:** Concludes each game, with wagers and answer judging
* **Score History & High Scores:** Visual score progression (Chart.js), persistent local high score tracking
* **Audio support:** Jeopardy music and correct/incorrect sound effects (toggleable)
* **Speech Synthesis:** Reads questions aloud (browser support required)
* **Responsive design:** Desktop and mobile optimized, print-friendly

---

## Installation & Deployment

### Prerequisites

* Modern web browser (Chrome, Edge, Firefox, Safari) with JavaScript enabled
* No server required; all functionality is client-side
* To enable full audio and speech features, ensure browser permissions for sound are granted

### Setup Steps

1. **File Placement:**
   Place `index.html` and all referenced assets in the same directory:

   * Audio files:

     * `Jeopardy - 2008 - Opening.mp3`
     * `sounds/correct.mp3`
     * `sounds/wrong.mp3`
     * `sounds/daily_double.mp3`
     * `sounds/final_jeopardy.mp3`
   * (Optional: Place these in a `sounds/` subdirectory if desired, as referenced in the code.)

2. **Open the Game:**
   Double-click `index.html` or open it via your preferred browser.

3. **Network Access:**
   No internet connection is required after initial asset download (except for loading Google Fonts and Chart.js from CDN).

---

## How to Play

1. **Add Players:**
   Enter player names and click "Add Player" for each participant (up to 8).

2. **Start Game:**
   Once all players are added, click "Start Game." The game board will appear.

3. **Select Questions:**
   Click on a question tile to reveal the question. The host will judge answers as "Correct" or "Wrong" and may reveal the answer at any time.

4. **Scorekeeping & Turn Rotation:**
   Scores update automatically. The host can manually adjust scores if necessary and rotate control if "Rotate Control" is enabled.

5. **Daily Double:**
   Randomly assigned; allows the active player to wager any amount (within limits).

6. **Final Jeopardy:**
   When all questions are answered, "Final Jeopardy" becomes available. Players make wagers, the question is revealed, and the host judges answers.

7. **Review History:**
   Use tabs for "Score History" (progression graph) and "High Scores" (persisted across sessions).

---

## Customization

* **Categories & Questions:**
  Questions are hardcoded in the JavaScript section for rapid deployment. To customize, modify the `gameData` and `questionBank` variables.

* **Audio/Visuals:**
  Replace audio files or edit CSS variables in the `<style>` block for different branding or corporate identity.

* **Accessibility:**
  Game is keyboard-accessible and readable via screen readers. Audio and speech functions are toggleable.

---

## Technical Notes

* **Persistence:**
  Game state and high scores are saved locally (browser LocalStorage). Clearing browser data will reset history and saved games.
* **No External Dependencies:**
  All logic is self-contained. Third-party libraries are loaded via CDN only for charting and fonts.
* **Security:**
  No data is sent or stored externally; all user data resides on the user’s machine.

---

## Maintenance

* To update questions, categories, or rules, modify the relevant sections in the `<script type="module">` tag.
* For further feature expansion (new categories, player limits, new round types), extend the `gameData`, `questionBank`, and related functions.
* For corporate deployment, host on an internal web server or learning management system as a static site.

---

## Credits

Developed for educational and professional training in food manufacturing environments by Stevo607.
Incorporates best practices in interactive learning for food safety, quality, and compliance.

---

## Support

For issues, enhancements, or additional deployment support, contact Stevo607 - stevo607@hotmail.com
---

**End of README**
