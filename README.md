# PayPol Protocol 🦞⚡

> **The Durable Financial OS for the Agentic Economy.**
>
> *Powered by Tempo. Integrated with OpenClaw. Built for Autonomous Money.*

[![OpenClaw Ready](https://img.shields.io/badge/OpenClaw-Compatible-FF4500?style=for-the-badge&logo=robot&logoColor=white)]()
[![Tempo Architecture](https://img.shields.io/badge/Workflow-Durable-000000?style=for-the-badge&logo=temporal&logoColor=white)]()
[![License: BSL 1.1](https://img.shields.io/badge/License-BSL%201.1-blue?style=for-the-badge)]()
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen?style=for-the-badge)]()

## 💡 The Manifesto

We are officially entering the age of **Autonomous AI agents**. Platforms like [OpenClaw](https://github.com/OpenClaw/OpenClaw) (The Lobster) now enable AI to handle sophisticated workflows such as writing code and managing deployments, yet these agents remain financially stranded. While typical crypto wallets present too many security risks for automated bots, conventional payment systems are simply too inflexible to meet their unique needs

**PayPol** is the missing link. We provide the "Financial OS" for AI Agents, enabling them to earn, spend, and manage assets securely via **Durable Workflows** on the [Tempo Blockchain](https://tempo.io/) 

**Why PayPol?**
* **For Humans:** Sleep soundly knowing your agents have strict limits and a "Panic Button".
* **For Agents:** True financial identity to subscribe to APIs, rent servers, or tip peers.
* **For Devs:** Workflow-as-Code. No more "pending transaction" nightmares.

---

## 🚀 6 Unique Capabilities

### 1. 🦞 Native "Agent Identity" Wallets
Stop giving your private keys to bots. PayPol creates **Ephemeral Sub-Wallets** for your agents.
* *Scenario:* You authorize your **OpenClaw** agent to rent a server.
* *PayPol:* Allocates a wallet with exactly $20 limit/day. If the agent goes rogue, your main vault remains untouched.

### 2. 💓 Heartbeat Payments (Pay-as-you-Live)
Agents have a heartbeat. We monetize it.
Configure your agent to stream payments (e.g., $0.001/min) to API providers only while it is active. If the agent crashes or sleeps, the payment stream stops instantly. Zero waste.

### 3. 🛡️ The "Lobster Trap" (Time-Vault Security)
Agents can be hallucinated or hijacked. PayPol protects your funds with a programmable **Time-Vault**.
* *Scenario:* Your agent tries to send $1000 to a suspicious address.
* *PayPol:* Holds funds for 15 minutes. Sends you a Telegram alert.
* *Action:* You hit the **PANIC BUTTON** on the dashboard → Transaction Reverted.

### 4. 🧠 Skill-Based Budgeting
Grant specific allowances to specific OpenClaw Skills via our policy engine.
* `skill-aws`: Limit $50/day (Infrastructure).
* `skill-twitter`: Limit $0/day (Social).
* *Result:* A compromised social skill cannot drain your infrastructure budget.

### 5. 🤝 The Moltbook Economy
Native tipping for the Agent Social Network.
Enable your agent to autonomously tip other agents on **Moltbook** for useful data, prompts, or collaboration, settling instantly on Tempo with near-zero gas.

### 6. ✅ Verifiable Output Payments (Merit Protocol)
Agents make mistakes. PayPol ensures you only pay for success.
Link your payments to external validators like GitHub Actions or "Critic Agents".
* *Scenario:* OpenClaw generates a bug fix.
* *PayPol:* Workflow waits for CI checks.
* *Action:* Funds released **if and only if** `npm test` passes (Green Build).
* *Result:* Zero cost for hallucinated code.

---

## 🗺️ The Grand Roadmap

We are building the financial infrastructure for the next decade of AI Autonomy.

### Phase 1: Genesis (The Shell) 🏗️
*Building the bedrock of the Agentic Economy on Tempo.*
* [ ] **Core Protocol:** Deploy `PayPol_v1` smart contracts on Tempo Mainnet for high-throughput, gas-optimized USDC settlement.
* [ ] **Agent Identity Standard:** Launch AIP-1 (Agent Identity Protocol) to assign unique, verifiable on-chain identities to OpenClaw instances.
* [ ] **PayPol CLI:** Release the command-line interface for developers to manage agent wallets manually (`paypol init`, `paypol balance`).
* [ ] **Basic Security:** Implementation of hard-capped spending limits per API key.

### Phase 2: Symbiosis (The Claw) 🦞
*Deep integration with the OpenClaw ecosystem.*
* [ ] **Native Skill Release:** Official `@paypol/skill` available on the OpenClaw registry. Enables agents to perform natural language financial actions ("Send $5 to @bob").
* [ ] **Heartbeat Billing Engine:** Launch the Micro-Payment Stream protocol. Services bill agents per block/second based on active "heartbeats".
* [ ] **The "Lobster Trap" (Beta):** Introduction of the 15-minute Time-Vault. Users can visualize pending agent transactions and manually revert them via a basic UI.

### Phase 3: Sentinel (The Shield) 🛡️
*Advanced AI-driven security and human-in-the-loop controls.*
* [ ] **Risk Engine v1:** Deploy ML models to detect anomaly patterns (e.g., an agent suddenly draining funds or interacting with blacklisted contracts).
* [ ] **Panic Button Dashboard:** A full-featured React Native mobile app for real-time monitoring and emergency "Kill Switch" activation.
* [ ] **Multi-Sig for Bots:** Require human approval (via Telegram/Slack) for any transaction exceeding a user-defined threshold (e.g., >$50).

### Phase 4: Colony (The Ocean) 🌊
*Expanding the economy to Agent-to-Agent (A2A) commerce.*
* [ ] **Moltbook Economy:** Native integration with the Moltbook social network. Enable "Like-to-Tip" and "Data-for-Cash" markets between agents.
* [ ] **Skill Marketplace:** A decentralized registry where developers can sell specialized OpenClaw skills (e.g., "Advanced Trading Strategy") directly to other agents.
* [ ] **Developer SDKs:** Release full-suite SDKs for Python, Node.js, and Go to embed PayPol into custom agent frameworks beyond OpenClaw.

### Phase 5: Singularity (The Leviathan) 🌌
*Full financial autonomy and cross-chain abstraction.*
* [ ] **Chain Abstraction Layer:** Agents simply pay in USDC; PayPol handles bridging to Ethereum, Solana, or Base in the background.
* [ ] **Autonomous Treasuries:** Enable DAOs managed entirely by a swarm of OpenClaw agents with voting rights based on reputation.
* [ ] **PayPol Network Decentralization:** Transitioning the "Risk Engine" and "Relayer" nodes to a decentralized community-run network.

---

## 🏗 System Architecture

PayPol is engineered as a high-performance Monorepo to ensure scalability and developer velocity.

```bash
paypol-protocol/
├── .github/
│   └── workflows/                     # CI/CD Pipelines (Auto-deploy to Hetzner)
├── .env.example                       # Environment Configuration Template
├── docker-compose.yml                 # Local Development Orchestration
├── Makefile                           # Shortcut Commands (make start, make deploy)
│
├── 📂 apps/                           # [Frontend Layer] Human Interaction Interfaces
│   ├── dashboard/                     # [Next.js] Command Center for Users
│   │   ├── src/app/
│   │   │   ├── agents/                # Agent Management & Limit Configuration
│   │   │   ├── panic/                 # 🚨 Panic Button UI (Emergency Reversal)
│   │   │   └── logs/                  # Real-time Agent Heartbeat Monitoring
│   │   └── Dockerfile
│   │
│   ├── mobile/                        # [React Native] iOS/Android Monitoring App
│   │   ├── src/screens/PanicScreen.tsx
│   │   └── src/screens/WalletDetail.tsx
│   │
│   └── docs/                          # [Docusaurus] Developer Hub
│       ├── docs/api/                  # API Reference
│       └── docs/skills/               # Integration Guides for OpenClaw
│
├── 📂 ecosystem/                      # [Integration Layer] External Plugins
│   ├── openclaw-skill/                # 🦞 Native Skill for OpenClaw Agents
│   │   ├── paypol_skill/
│   │   │   ├── manifest.json          # Permission Scopes & Capabilities
│   │   │   └── tools.py               # Logic: execute_payment(), check_limit()
│   │   └── README.md                  # Installation: "pip install paypol-skill"
│   │
│   └── github-action/                 # ✅ Merit Pay Protocol (Feature 6)
│       ├── action.yml                 # CI/CD Integration
│       └── src/index.js               # Trigger Fund Release on "Green Build"
│
├── 📂 services/                       # [Backend Layer] Core Microservices
│   ├── api-gateway/                   # [Nginx] Entrypoint & Rate Limiting
│   │   └── nginx.conf
│   │
│   ├── tempo-workers/                 # 🧠 [Python] Durable Execution Engine (The Brain)
│   │   ├── src/
│   │   │   ├── workflows/             # Business Logic & State Machines
│   │   │   │   ├── payment_flow.py    # Standard Transfer Logic
│   │   │   │   ├── escrow_flow.py     # Conditional Release Logic
│   │   │   │   └── lobster_trap.py    # The "Lobster Trap" (15m Time-Lock)
│   │   │   └── activities/            # Atomic Tasks & Side Effects
│   │   │       ├── blockchain.py      # On-chain Tempo Interactions
│   │   │       ├── notification.py    # Telegram/Slack Alerts
│   │   │       └── verifier.py        # CI/CD Status Verification
│   │   └── Dockerfile
│   │
│   ├── risk-engine/                   # 🛡️ [ML] Anomaly Detection System
│   │   ├── model/                     # Pre-trained Fraud Detection Models
│   │   └── policy/                    # Hard Rules (e.g., Max $50/day)
│   │
│   └── agent-auth/                    # Identity Provider (API Key -> Wallet)
│       └── src/routes/auth.py
│
├── 📂 packages/                       # [Shared Layer] Libraries & Contracts
│   ├── contracts/                     # 📜 Tempo Smart Contracts (Solidity)
│   │   ├── src/
│   │   │   ├── AgentWallet.sol        # Identity-bound Wallet Logic
│   │   │   ├── TimeVault.sol          # Programmable Time-Lock (Feature 3)
│   │   │   └── MeritPay.sol           # Output-Verification Logic (Feature 6)
│   │   └── foundry.toml               # Blockchain Development Config
│   │
│   ├── sdk/                           # Universal Client Libraries
│   │   ├── python/                    # `pip install paypol-sdk`
│   │   └── typescript/                # `npm install @paypol/sdk`
│   │
│   └── database/                      # Data Persistence Layer
│       ├── migrations/                # SQL Schema Migrations
│       └── schema.prisma              # Object-Relational Mapping
│
└── 📂 infra/                          # [DevOps Layer] Infrastructure as Code
    ├── hetzner/                       # Cloud Provisioning Scripts
    ├── tempo-node/                    # Custom RPC Node Configuration
    └── monitoring/                    # Grafana/Prometheus Dashboards
```

---

## 🛠 Tech Stack
* Orchestration: [Tempo](https://tempo.io/) (Durable Execution)
* Agent Framework: [OpenClaw](https://github.com/OpenClaw/OpenClaw)
* Backend: Python 3.11 (FastAPI)
* Database: PostgreSQL (TimescaleDB for ledger)
* Infrastructure: Docker, Hetzner Cloud

---

## ⚡ Getting Started

### Prerequisites

* Docker & Docker Compose
* Python 3.11+
* Node.js 20+

### Quick Start (Dev Mode)

1. Clone the Repo

   ```bash
   git clone [https://github.com/PayPol-Foundation/paypol-protocol.git](https://github.com/PayPol-Foundation/paypol-protocol.git)
   cd paypol-protocol
   ```
2. Launch the Stack

   ```bash
   docker compose up -d
   ```
   * Dashboard: http://localhost:3000
   * API Core: http://localhost:8000
     
3. Run the Worker

   ```bash
   cd services/tempo-workers
   python worker.py
   ```
   
## 📜 License & Copyright

Business Source License 1.1 (BSL)

The source code is available for use in non-production or for development/testing purposes.
Production use is allowed only for personal projects or entities with less than $1M in revenue.
For commercial licenses, please contact the PayPol Foundation.

Standard Open Source (MIT/Apache) conversion date: TBD (2 years from release)



<p align="center">
<i>Built with ❤️ by the PayPol Team.</i>

    
</p>
