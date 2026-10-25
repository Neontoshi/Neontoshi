# Hey, I'm Neon 👋

> **"I build things that push boundaries from cross-platform apps and blockchain-powered fairness engines, to CLI powerhouse tools."**

I'm a full-stack developer working at the intersection of **Rust**, **TypeScript**, and **systems engineering**. I build software that's fast, correct, and a little unconventional from music players with custom audio pipelines to provably fair systems on Solana.

---

## What I'm Building Right Now

### 🎵 [Kyma](https://github.com/neontoshi/Kyma)
**Cross-platform music player with a custom audio pipeline**
- **Stack:** Tauri, Rust, TypeScript, React
- **Audio Engine:** Symphonia (decoding) + CPAL (playback) - full control over the audio pipeline, down to a custom `HttpReader` with real HTTP range-request seeking
- **Streaming:** YouTube/SoundCloud playback with automatic stream-URL re-resolution as CDN links expire, TTL-based caching shared across both sources
- **Visuals:** Butterchurn visualizer with preset sync and freeze-on-pause behavior
- **Why it matters:** Most music players are wrappers around webviews. Kyma is native audio, end-to-end.
- **Status:** Actively developed across multiple builds; core playback pipeline stable

### 🛍️ [Shopcore](https://github.com/neontoshi/shopcore)
**E-commerce backend with Rust/Axum - built for scale**
- **Stack:** Rust, Axum, PostgreSQL (SQLx), Redis, TypeScript/Vite frontend
- **Payments:** Stripe (with HMAC-verified webhooks) plus crypto payments via NOWPayments
- **Auth:** Role-based access control with a proper `UserRole` type instead of raw strings, Redis-backed sessions
- **Features:** Full storefront + admin dashboard, cart, checkout, address management, order lifecycle
- **Why it matters:** Most e-commerce backends are Node.js/Python. Shopcore is built with Rust. faster, safer, cheaper to run.
- **Status:** MVP ready, multi-tenant support in progress

### 📬 [Huggmailer](https://github.com/neontoshi/huggmailer)
**Automated job-application email pipeline as a desktop app**
- **Stack:** Tauri, Rust, TypeScript/React
- **Features:** Multi-provider AI email generation (OpenAI, Groq, Gemini, DeepSeek, Grok), custom-designed PDF cover letters and email templates, JWT + API-key auth, Redis-backed rate limiting
- **Why it matters:** Email automation without the bloat. Lightweight, configurable, Rust-native, and it auto-provisions its own headless browser at build time.
- **Status:** Production ready

### 💬 [NeonWhat](https://github.com/Neontoshi/neon-wha)
**A native Linux desktop client for WhatsApp, in about 5 MB**
- **Stack:** Tauri 2, Rust, WebKitGTK
- **Native Integration:** OS notifications routed from WhatsApp Web's browser notifications, a system tray icon with a live unread badge, close-to-tray, and a global `Ctrl+Shift+W` show/hide shortcut
- **Under the Hood:** Injected JS bridges notifications and tracks unread counts from the page title, a Chrome user-agent spoof keeps WhatsApp Web working on WebKitGTK, and custom CSS themes load from a local config folder
- **Why it matters:** There's no official WhatsApp app for Linux, and most wrappers ship a full Chromium. NeonWhat uses the system webview, so it stays tiny.
- **Status:** Actively developed

### 🎲 [Provable-Fairness-Engine](https://github.com/neontoshi/provable-fairness-engine)
**A provably fair selection system on Solana**
- **Stack:** Rust, Solana, Anchor, Axum, PostgreSQL
- **The Problem:** How do you run a fair raffle/giveaway where even the organizer can't cheat?
- **The Solution:** Commit-reveal randomness sourced from on-chain `SlotHashes` and hashed with keccak — the outcome is derived on-chain and independently verifiable, not chosen by anyone.
- **Why it matters:** Trustless systems are the future. No central authority, no manipulation.
- **Status:** Deployed to devnet, on-chain verification UI in progress

### 🔍 [Code-Intelligence](https://github.com/neontoshi/code-intelligence)
**Multi-language static analysis for dead code, duplicate detection, and call graphs**
- **Stack:** Rust, Tree-sitter, ML (logistic regression), LLM integration
- **Languages:** Rust, Python, TypeScript/JS, Go, Java, Dart, PHP, C++, C# (10+ languages)
- **Features:**
  - Dead code detection via ML + graph reachability over a `petgraph` call graph
  - Structural duplicate detection (MinHash + LSH + ML pair classification)
  - Interactive Graphviz call-graph visualization
  - LLM-powered code summaries (Ollama, OpenAI, and Anthropic support in progress)
- **Why it matters:** Most static analysis tools are language-specific. Code-Intelligence is polyglot and fast.
- **Status:** Actively developed core analysis pipeline works end-to-end on real multi-language codebases; hardening test coverage and edge cases

---

## My Stack

| Layer | Technologies |
|-------|--------------|
| **Languages** | Rust, TypeScript, Python |
| **Frontend** | React, Tauri |
| **Backend** | Axum, Tokio |
| **Databases** | PostgreSQL, Redis, SQLite |
| **Blockchain** | Solana, Anchor |
| **Tooling** | Cargo, pnpm, Docker, GitHub Actions |

---

## Find Me Here
- **GitHub:** [neontoshi](https://github.com/neontoshi)
- **LinkedIn:** [daisi-samuel](https://www.linkedin.com/in/daisi-samuel)
- **Email:** [kidblip1@gmail.com](mailto:kidblip1@gmail.com)

---

## Philosophy

> "Code is not just instructions, it's a system. I build systems that are fast, correct, and fair."

---

*Currently deep in the Rust trenches, building the next generation of developer tooling.* 🦀
