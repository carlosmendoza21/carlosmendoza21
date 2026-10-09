### Hi, I'm Carlos Mendoza 👋

**Computer Science graduate in Houston, TX, building backend systems, ML applications, and real-time software.**

🤝 Open to roles in **ML engineering**, **backend engineering**, or **full-stack**, especially on teams working on applied AI.

---

### 🛠 Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat&logo=three.js&logoColor=white)

**Focus areas** · Reinforcement learning · REST APIs · Real-time systems · Model training & deployment

---

### 🚀 Featured projects

**[Deadlock Live Odds](https://github.com/carlosmendoza21/Deadlock-Dashboard)**: Live win-probability dashboard for Valve's *Deadlock*. Look up any player to see their current match with a chance-to-win that updates as souls and objectives change.
- Logistic-regression model fitted on ~25,000 real matches, with separate models at each game-time checkpoint
- Held-out accuracy climbs from **60% pre-game** to **83% at 35 min**, and predicted odds stay well calibrated
- Found and fixed a target leak (rank badges that already included the match result) that had inflated the rank effect ~10×
- Live backtesting harness that scores the app's real predictions with Brier score, log loss, and calibration

`TypeScript` `React` `Vite` `Logistic regression` `REST API`

**[Chromophobia](https://chromophobia.vercel.app)** · [repo](https://github.com/carlosmendoza21/chromophobia): Real-time music visualizer that reacts to Spotify playback with retro-styled WebGL visuals, live audio analysis via Meyda.js, and an AI mood classifier (Happy / Sad / Energetic / Angry) powered by a random forest model and served over WebSocket. Built as a 7-person senior project at UHCL.

`React` `Three.js` `Python` `PyTorch` `Meyda.js` `Spotify API` `Node.js`

**c-server** *(private, in progress)*: HTTP/1.1 server written from scratch in C on raw POSIX sockets, with no libraries or frameworks.
- Buffered request reading that loops until the end of the headers, with size caps and per-client read timeouts
- Request-line parsing, routing with 404 handling, and graceful handling of dropped clients (`SIGPIPE`, `EINTR`)

`C` `POSIX sockets` `HTTP` `CMake`

---

### 🎓 Background

BS in Computer Science · University of Houston – Clear Lake · 2026

