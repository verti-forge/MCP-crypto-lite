# 🧠 MCP Crypto-Lite  

A minimal, modular crypto trading bot built with Node + TypeScript + MCP.
Paper-trading foundation ready for Hyperliquid testnet integration.

🚀 Overview

This project establishes a clean foundation for a multi-phase crypto bot system using the Model Context Protocol (MCP) framework.
It currently runs in paper mode — executing mock trades and verifying logic before connecting to real exchanges.

Phase	Status	Description
1. MCP Server Foundation	✅ Complete	Paper trading, ping/ticker/order tools verified
2. Hyperliquid Testnet Integration	⏳ Next	Replace mocks with live API + WebSocket support
3. Signal Generation & Routing	🔜	Implements 105k / 117k zone strategies
4. Policy & Risk Management	🔜	Guardrails: max risk, daily loss caps
5. Coach Mode & Logging	🔜	Trade reasoning, Telegram alerts
6. State Persistence & Recovery	🔜	Full restart recovery & PnL tracking
🧩 Project Structure
mcp-crypto-lite/
├── data/
│   └── .gitkeep              # keeps data dir but ignores runtime JSON
├── src/
│   ├── env.ts                # environment loader
│   ├── server.ts             # MCP entry point
│   ├── tools/
│   │   ├── ping.ts
│   │   ├── getTicker.ts
│   │   └── placeOrder.ts
│   └── services/
│       └── hyperliquid.ts    # exchange adapter (stub)
├── .env.example              # template for safe environment variables
├── .gitignore
├── package.json
├── tsconfig.json
└── README.md

⚙️ Setup & Run
1. Install dependencies
npm install

2. Run server in dev mode
npm run dev

3. Run local test script
npm test


You’ll see three test confirmations:

✅ Ping tool success

✅ Get-ticker success

✅ Paper order written to data/orders.json

🔒 Environment Variables

Copy .env.example → .env and fill in:

HL_BASE=https://api.hyperliquid-testnet.xyz
HL_AGENT_WALLET=<your-testnet-agent-address>
HL_AGENT_KEY=<private-key-testnet-only>

🧱 Tech Stack

Node.js 22+

TypeScript 5

MCP SDK

ts-node

dotenv

🧭 Design Philosophy

Automation builds the walls; ChainScope makes the windows.

This repo follows the optional-truth ethos — safe, transparent, and easily extensible.
Every phase builds toward a modular agent environment capable of real-time trading, risk control, and contextual reasoning.

🧩 Next Phase (2): Hyperliquid Integration

Replace mock price data with live API fetch

Implement WebSocket subscriptions

Verify order placement on testnet

🪄 Credits

Built by Travis Buck (@TravisWooWealth
)
Guided by the MCP Stack and ChainScope development philosophy.
