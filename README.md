# Mouse Practice Game

**Note:** Just a heads-up! This game was created as a fun vibe coding exercise during free time. Hope you find it useful (and fun)!

A simple web-based game designed to help users practice mouse accuracy, reaction time, and clicking speed.

## Features

* **Target Clicking:** Click randomly appearing circular targets within the game area. Targets spawn intelligently to avoid overlapping.
* **Immediate Respawn:** When the screen is clear during gameplay, a new target appears instantly for continuous action.
* **Scoring:** Earn points for each target successfully clicked.
* **Accuracy Tracking:** Monitors your click accuracy (hits vs. total clicks).
* **Hit Rate Tracking:** See the percentage of spawned targets that you successfully hit.
* **Reaction Time:** Measures the time it takes you to click a target after it appears (shown for hits).
* **Timed Sessions:** Play rounds for a configurable duration with a visible countdown timer (turns red in the last 10 seconds).
* **Difficulty Presets:** Choose from predefined difficulties (Easy, Normal, Hard, Veteran, Aimbot) or use Custom settings. Presets adjust spawn rate, target lifetime, and max targets.
* **Configurable Difficulty:** Manually adjust settings like:
    * Target spawn rate (minimum and maximum time between spawns).
    * Target lifetime (how long targets stay on screen).
    * Maximum number of targets on screen at once.
    * Game duration per session (independent of difficulty presets).
* **Pause/Resume:** Pause the game at any time using the 'P' key.
* **Summary Screen:** View your score and accuracy at the end of each timed session.
* **Replay Options:** After a session, choose to play again immediately (keeping current settings) or return to the start screen.
* **Game History:** View the results (score, accuracy, date) of your last 10 completed sessions, filterable by the difficulty preset used for that session.
* **Persistent Settings:** Your configuration settings (including selected preset or custom values, and game duration) are saved in your browser via `localStorage`, so they'll be remembered the next time you play.

## Offline Capability & Safety

* **Offline Play:** Once the game page is loaded, it runs entirely in your browser and does not require an active internet connection to play.
* **Data Storage:** Configuration settings and game history (separated by difficulty) are stored locally in *your browser's* `localStorage`. This data is not sent anywhere.
* **Safety:** The game is built using standard HTML, CSS, and JavaScript. It does **not** load external scripts, and the code operates entirely within the confines and security sandbox of your browser tab.

## How to Play

1.  Load the `index.html` file (or the page where it's hosted) in your web browser. Your previous settings will be loaded automatically if available.
2.  (Optional) Click the "Settings" button. You can either:
    * Click a Difficulty Preset button (Easy, Normal, etc.) to load standard settings.
    * Manually adjust the individual sliders. If your settings don't match a preset, the "Custom" button will become active. You can also click "Custom" to keep your current manual settings active.
    * Adjust the "Game Duration".
    * Click "Apply & Close" to save your configuration for future sessions.
3.  Click the "Play" button that appears over the game area.
4.  Targets will start appearing. Click them as quickly and accurately as possible.
5.  The game runs for the configured duration. Keep an eye on the "Time Left" display (it turns red near the end).
6.  Press 'P' to pause or resume the game (cannot pause while modals are open).
7.  During active gameplay (when not paused), click the "Reset" button (top bar) or press 'R' to stop the current round immediately and reset stats (your configuration settings are kept).
8.  When the time runs out, a summary screen will show your results for that session.
9.  From the summary screen:
    * Click "Play Again Immediately" to start another round instantly using the same settings you just played with.
    * Click "Back to Start" to return to the initial screen (keeping your settings); you'll need to press "Play" again.
10. Click the "History" button (top bar) when the game is stopped to view your recent session results. Use the dropdown menu in the history panel to view results for different difficulty presets.

## Known Issues

* **Accuracy/Hit Rate Calculation:** The Accuracy and Hit Rate percentages may display incorrect values (e.g., starting at 50% or 500%) after the first few interactions, especially after hitting the first target. This relates to how initial clicks are counted.
