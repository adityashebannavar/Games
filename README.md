# 🎯 Wordlerz - Full-Stack Multiplayer & Solo Word Similarity Game

A complete, production-ready full-stack word similarity guessing game. Built with **Node.js, Express, Socket.io, and modern HTML5/Canvas/CSS3**.

---

## ✨ Features

### 1. 🏠 Clean Home Server
- **Zero clutter on home**: No overwhelming settings.
- **Customizable Avatar**: 12 expressive gamer & character avatars with gradient badges.
- **Player Name Input**: Stored across sessions.
- **Game Mode Selection**:
  - 🧠 **Solo Mode**
  - 👥 **Multiplayer Mode**
- Big **PLAY NOW 🚀** button directing to the chosen server mode.

### 2. 🧠 Solo Mode (`/solo`)
- **Separate Server Instance & State**: Dedicated game session.
- **Semantic Distance Closeness**:
  - 🟢 **Green (Rank 1 - 500)**: Very close / immediate semantic domain.
  - 🟠 **Orange (Rank 501 - 1000)**: Close / getting warm.
  - 🔴 **Red (Rank > 1000)**: Cold / far away.
  - ⭐ **Rank 1**: The exact secret word!
- **Contexto Visual Progress Bars**: Color-coded, animated progress bars showing similarity percentage and rank numbers.
- **Clue & Hint System**:
  - Clues by category, physical nature, color, shape, and characteristics.
  - Revealing closer candidate words to guide players.
  - Real-time guess count and hints count tracker.
- **Victory Celebration**:
  - Confetti explosion animation via custom Canvas engine.
  - Synthesized Web Audio fanfare.
  - Victory modal displaying secret word, time taken in seconds, total guesses, and hints used.

### 3. 👥 Multiplayer Mode (`/multiplayer`)
- **Dialog Selection**:
  - 👑 **Create Room**: Create a private party room with a 6-character code.
  - 🔑 **Join Private Room**: Enter party code to join friends.
  - 🌍 **Join Random Game**: Instant matchmaker with open public rooms worldwide.
- **Multiplayer Lobby**:
  - Party code display with 1-click clipboard copy.
  - Live player count indicator (e.g. `2 / 8`).
  - Player list showing their selected avatar and name, plus host badge.
  - **Live Chatting Box**: Real-time chatting between players (strictly human, **NO BOTS**).
  - **Admin / Host Controls**:
    - Customize maximum players (4, 8, 12, 16).
    - Customize number of rounds (1, 3, 5).
    - Choose points system (Standard 100 pts vs Speed Bonus).
    - Only the Admin / Host has the **"START GAME"** button.
  - **Normal Player View**: Clean waiting notice while host configures the game.
- **In-Game Multiplayer Match**:
  - Synchronized round gameplay with secret word for all players.
  - Contexto guess board for each player's private guesses.
  - **Real-Time Live Leaderboard**: Displays all players' best ranks, total guesses, and cumulative match points live as they submit guesses.
  - **In-Game Live Chat Drawer**: Chat live during rounds.
  - **Round End Celebration**:
    - Triggered immediately when any player guesses Rank 1.
    - Confetti on all players' screens!
    - Winner announcement modal with time taken and guess counts.
    - Admin can proceed to the next round with 1 click.
    - Final match podium celebration on the last round.

---

## 🚀 Running the Game

1. Double-click `start.bat`, or in terminal run:
   ```bash
   node server/index.js
   ```
2. Open your browser:
   - **Home**: [http://localhost:3000](http://localhost:3000)
   - **Solo Mode**: [http://localhost:3000/solo](http://localhost:3000/solo)
   - **Multiplayer Mode**: [http://localhost:3000/multiplayer](http://localhost:3000/multiplayer)
