### Hi, I'm Carlos Mendoza

**Computer Science graduate in Houston, TX, building backend systems, ML applications, and real-time software.**

Open to roles in **ML engineering**, **backend engineering**, or **full-stack**, especially on teams working on applied AI.

---

### Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat&logo=cmake&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat&logo=three.js&logoColor=white)

**Focus areas**: Reinforcement learning, REST APIs, real-time systems, systems programming, model training and deployment

---

### Featured projects

**[Deadlock Dashboard](https://github.com/carlosmendoza21/Deadlock-Dashboard)**: Live win-probability dashboard for Valve's *Deadlock*. Look up any player to see their current match with a chance-to-win that updates as souls and objectives change.
- Logistic-regression model fitted on ~25,000 real matches, with separate models at each game-time checkpoint
- Held-out accuracy climbs from **60% pre-game** to **83% at 35 min**, and predicted odds stay well calibrated
- Found and fixed a target leak (rank badges that already included the match result) that had inflated the rank effect ~10x
- Live backtesting harness that scores the app's real predictions with Brier score, log loss, and calibration

`TypeScript` `React` `Vite` `Logistic regression` `REST API`

**[c-server](https://github.com/carlosmendoza21/c-server)** *(in progress)*: HTTP/1.1 server written from scratch in C on raw POSIX sockets, with no libraries or frameworks.
- Persistent accept loop that reads full requests with an 8 KB size cap and a 5-second receive timeout
- Request-line parsing and path-based responses, with proper `400`, `404`, `405`, `408`, and `431` error responses
- Reliable writes (`send_all`) and graceful handling of dropped clients (`SIGPIPE`)
- Next up: concurrency (thread pool / epoll), keep-alive, static file serving, benchmarks, and a test suite

`C` `POSIX sockets` `HTTP` `CMake`

**[emberkv](https://github.com/carlosmendoza21/emberkv)** *(just started)*: A Redis-style in-memory key-value store in modern C++, with a command parser, a server/REPL executable, and GoogleTest unit tests. Builds with strict compiler warnings and optional AddressSanitizer / ThreadSanitizer / UBSan.

`C++20` `CMake` `GoogleTest`

**[Chromophobia](https://chromophobia.vercel.app)** ([repo](https://github.com/carlosmendoza21/chromophobia)): Real-time music visualizer that reacts to Spotify playback with retro-styled WebGL visuals, live audio analysis via Meyda.js, and an AI mood classifier (Happy / Sad / Energetic / Angry) powered by a random forest classifier and served over WebSocket. Built as a 7-person senior project at UHCL.

`React` `Three.js` `Python` `PyTorch` `Meyda.js` `Spotify API` `Node.js`

---

### Background

BS in Computer Science, University of Houston - Clear Lake, 2026
