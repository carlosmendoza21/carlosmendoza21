### Hi, I'm Carlos Mendoza

**Computer Science graduate in Houston, TX, building backend systems, ML applications, and real-time software.**

Open to roles in **ML engineering**, **backend engineering**, or **full-stack**, especially on teams working on applied AI.

---

### Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=black)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat&logo=cmake&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat&logo=three.js&logoColor=white)

**Focus areas**: Backend APIs, data pipelines, applied ML, real-time systems, systems programming

---

### Featured projects

**osu! AI Coach** *(in progress)* · [Repo](https://github.com/carlosmendoza21/osu-coach)

Analyzes osu! replays hit by hit, builds a skill profile (aim, speed, accuracy, consistency, stamina, reading), and recommends practice maps that target a player's weak spots.
- FastAPI backend with Celery workers, PostgreSQL 16 + pgvector, and Redis, all running with one `docker compose up`
- osu! API v2 client with a cached OAuth token, a shared Redis rate limiter, and retries with exponential backoff and jitter that respect `Retry-After`
- `GET /players/{username}` syncs a player's profile and top/recent plays in a background worker, and falls back to stored data if osu! is down
- 277 unit tests (mocked HTTP, fake Redis, fake clock) plus Postgres integration tests in CI; strict `mypy` and `ruff`
- Next up: replay parsing, skill-profile model, map recommendations, and an LLM coach that explains weaknesses

`Python` `FastAPI` `PostgreSQL` `pgvector` `Redis` `Celery` `SQLAlchemy` `Docker` `GitHub Actions`

**Deadlock Dashboard** · [Live site](https://deadlockdashboard.vercel.app) · [Repo](https://github.com/carlosmendoza21/Deadlock-Dashboard)

Live win-probability dashboard for Valve's *Deadlock*. Look up any player to see their current match with a chance-to-win that updates as souls and objectives change.
- Logistic-regression model fitted on ~25,000 real matches, with separate models at each game-time checkpoint
- Held-out accuracy climbs from **60% pre-game** to **83% at 35 min**, and predicted odds stay well calibrated
- Found and fixed a target leak (rank badges that already included the match result) that had inflated the rank effect ~10x
- Live backtesting harness that scores the app's real predictions with Brier score, log loss, and calibration

`TypeScript` `React` `Vite` `Logistic regression` `REST API`

**Chromophobia** · [Live site](https://chromophobia.vercel.app) · [Repo](https://github.com/carlosmendoza21/chromophobia)

Real-time music visualizer that reacts to Spotify playback with retro-styled WebGL visuals, live audio analysis via Meyda.js, and an AI mood classifier (Happy / Sad / Energetic / Angry) powered by a random forest classifier and served over WebSocket. Built as a 7-person senior project at UHCL.

`React` `Three.js` `Python` `PyTorch` `Meyda.js` `Spotify API` `Node.js`

**c-server** *(in progress)* · [Repo](https://github.com/carlosmendoza21/c-server)

HTTP/1.1 static file server written from scratch in C on raw POSIX sockets, with no libraries or frameworks.
- Reads full requests across TCP segments, with an 8 KB header cap and a 5-second timeout so slow or oversized clients can't hang the server
- Streams files in 8 KB chunks with `Content-Type` picked from the file extension
- Three-layer path traversal protection (leading `/`, `..` segments, `realpath()` containment) that also blocks symlink escapes
- Correct `400`, `403`, `404`, `405`, `408`, `414`, `431`, and `500` responses
- 95 automated checks (C unit tests plus a live-server integration suite) run under AddressSanitizer with CTest
- Next up: `sendfile()`, keep-alive, and concurrency with `epoll` and multi-core workers

`C` `POSIX sockets` `HTTP` `CMake` `CTest`

---

### Background

BS in Computer Science, University of Houston - Clear Lake, 2026
