# 4th Grade Spelling Practice App 🎓

A fun, interactive, and colorful web-based spelling game designed for 4th graders. This single-page application features text-to-speech, gamified feedback (confetti, emojis), and a "smart" retry system that helps students master tricky words.

## 🎮 Features

* **Interactive Dashboard:** A "one-screen" layout designed to fit perfectly on laptops and tablets without scrolling.
* **Text-to-Speech (TTS):** Uses ResponsiveVoice.js to speak the words aloud to the student.
* **Visual Cues:** Dynamic emojis change based on the word being asked (e.g., "coward" shows a 🐔).
* **Smart Retry System:** Words missed during the game are added to a "Retry List." The game doesn't end until the student masters these specific words in a second round.
* **Top 5 Scoreboard:** Saves the fastest times locally in the browser to challenge the student.
* **Fun Feedback:** Confetti explosions for correct answers, sound effects, and encouraging voice lines.
* **Profanity Filter:** Built-in safety check for user names.

## 📁 Critical Setup Requirement: Asset Folders

**⚠️ IMPORTANT:** This game requires specific audio and image files to function correctly. The HTML code references a local `sounds` folder and an `images` folder.

If these folders do not exist, the game will still run, but you will not hear sound effects (ding/buzz/cheer) and the browser tab icon will be missing.

### Directory Structure
Ensure your project folder looks exactly like this:

```text
/project-folder
│
├── index.html          <-- The main game code
│
├── images/
│   └── favicon.png     <-- Browser tab icon
│
└── sounds/             <-- REQUIRED for audio feedback
    ├── button-3.mp3    (Sound for correct answer)
    ├── button-10.mp3   (Sound for incorrect answer)
    └── cheer.mp3       (Sound for game completion)
