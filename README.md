# 🧠 MCP Crypto-Lite

> **A minimal, modular crypto trading bot built with Node.js + TypeScript + MCP.**  
> Paper-trading foundation ready for **Hyperliquid Testnet** integration.

---

## 🚀 Overview

This project establishes a clean foundation for a multi-phase crypto-bot system using the **Model Context Protocol (MCP)** framework.  
It currently runs in paper mode — executing mock trades and verifying logic before connecting to real exchanges.

---

## 🧩 Roadmap

> Each phase builds toward a self-regulating trading agent capable of transparent, on-chain performance tracking.

| Phase | Goal | Key Milestones |
|:------|:------|:---------------|
| **2. Hyperliquid Testnet Integration** | 🔗 Replace mocks with live data | REST & WebSocket ticker stream, paper orders via testnet |
| **3. Signal Generation & Routing** | 🧠 Strategy logic | 105k / 117k zone detection, ATR-based confirmation router |
| **4. Policy & Risk Management** | 🛡️ Guardrails | Risk per trade, daily loss caps, trade cooldowns |
| **5. Coach Mode & Logging** | 🗣️ Contextual feedback | Telegram alerts, trade reasoning, structured journaling |
| **6. State Persistence & Recovery** | ♻️ Fault tolerance | Restart recovery, daily PnL tracking, persistent bot state |

---

## 🧾 Versioning & Conventions

- **TypeScript strict mode** enforced  
- **ESM modules** (Node 22+ compatible)  
- **Environment isolation:** `.env` and `.env.example`  
- **Paper-trading safety:** no real funds, full local state logging  

---

## 🤝 Contributing

Pull requests are welcome!  

---

## 🪪 License

MIT License — feel free to fork, modify, and build upon this foundation.

---

## 🧭 Project Ethos

Built with a focus on **clarity, safety, and transparency.**  
Every trade, decision, and state update is intended to be verifiable and human-auditable — aligning with the broader **Proof-of-Intent** philosophy.
