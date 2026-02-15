<div align="center">
  <img src="./apps/dashboard/paypol-frontend/public/logo.png" alt="PayPol Logo" width="160" />
  
  # PayPol OS

  **THE FINANCIAL OS FOR THE AGENTIC ECONOMY.**
  <br/>
  *Powered by [Tempo](https://tempo.xyz/) & [OpenClaw](https://openclaw.ai/)*

  [![License: BSL 1.1](https://img.shields.io/badge/License-BSL_1.1-red.svg)](https://mariadb.com/bsl11/)
  [![Tempo Network](https://img.shields.io/badge/Network-Tempo_Moderato-blueviolet.svg)](https://tempo.xyz)
  [![Architecture](https://img.shields.io/badge/Architecture-Multi--Tenant_SaaS-success.svg)]()
  [![Web3](https://img.shields.io/badge/Web3-EVM_Compatible-blue.svg)]()
  [![Privacy: Noir ZK](https://img.shields.io/badge/Privacy-Noir_ZK--Engine-black.svg)]()
</div>

---

## 🌌 Overview

**PayPol** is a monolithic, enterprise-grade Web3 Financial Operating System. Designed for DAOs, decentralized startups, and modern enterprises, PayPol bridges the gap between trustless decentralized finance (DeFi) and traditional corporate treasury management. 

Built natively on the high-performance **Tempo** and integrated with **OpenClaw** for agentic automation, PayPol transforms how organizations manage, secure, and dispatch on-chain liquidity.

---

## 🎯 10 Strategic Use Cases

PayPol is a full-lifecycle organizational primitive for the decentralized era:

1. **Automated Mass Payroll (Live):** Dispatch bulk stablecoin transactions with CSV routing.
2. **Multi-Sig Boardroom Security (Live):** EIP-191 signature enforcement for all treasury movements.
3. **Phantom Shield (Premium Privacy):** Optional ZK-Rollup feature to completely mask transaction amounts on the public ledger, protecting corporate salary data from competitors.
4. **Token Vesting & Cliff Unlocks:** Programmatic lock-ups for founders and early contributors.
5. **DAO Milestone Bounties:** Escrow-based grant distributions tied to Git or consensus triggers.
6. **Cross-Border B2B Invoicing:** Seamless Web3 billing for global contractors.
7. **Idle Treasury Yield Farming:** Route vaulted assets into DeFi protocols to earn yield.
8. **Algorithmic Tax Withholding:** Instant escrow of tax percentages during distributions.
9. **AI-Driven Expense Auditing:** OpenClaw AI agents autonomously verify invoices.
10. **Crypto-to-Fiat On/Off Ramping:** Built-in gateway for direct-to-bank settlement

---

## 🗺️ Strategic Roadmap

Our vision is to build the ultimate infrastructure for autonomous money across a 5-phase rollout.

### Phase 1: Foundation & Core Payroll 
- ✅ **Multi-Tenant SaaS Gateway (Genesis Workspace Setup)**
- ✅ **The Boardroom: Multi-Sig EIP-191 Authentication**
- ✅ **Agentic Autopilot for Recurring Payments**
- ✅ **Smart CSV Bulk Dispatch with Address Book Harvest**
- ✅ **One-Click Tax & Accounting Ledger Export**
- ✅ **Multi-Token Tempo Treasury (`AlphaUSD`, `pathUSD`, `BetaUSD`, `ThetaUSD`)**

### Phase 2: Advanced Treasury Yield & Privacy (Current)
- [ ] ZK-Proof Encryption for Hidden Salary Amounts (Use Case 3)
- [ ] Integration of Idle Treasury Yield Generation (Use Case 7)
- [ ] Cross-chain stablecoin swapping via OpenClaw Routing
- [ ] Granular Role-Based Access Control (RBAC) for HR and Mid-level Managers
- [ ] Advanced Financial Analytics & Burn Rate Dashboards

### Phase 3: Organizational Primitives 
- [ ] Token Vesting Contracts & Cliff Management (Use Case 4)
- [ ] Web3 Invoicing System for B2B Contractors (Use Case 6)
- [ ] Decentralized Identity (DID) integration for employee KYC/KYB
- [ ] Multi-Vault support (Segregating Marketing, Dev, and Ops funds)

### Phase 4: Fiat Integration & Compliance 
- [ ] Algorithmic Tax Withholding & Smart Escrow (Use Case 8)
- [ ] Real-time Crypto-to-Fiat Off-ramp API integration (Use Case 10)
- [ ] Automated generation of W-8BEN / W-9 equivalent Web3 tax forms
- [ ] Enterprise API endpoints for QuickBooks and Xero syncing

### Phase 5: The Fully Agentic Economy 
- [ ] DAO Bounties & Automated GitHub Escrow (Use Case 5)
- [ ] AI-Driven Expense Auditing & Micro-reimbursements (Use Case 9)
- [ ] Fully Autonomous OpenClaw AI for predictive treasury and risk management
- [ ] Public SDK for third-party dApp integrations

---

## 🏗️ System Architecture

PayPol operates on a **Multi-Tenant SaaS Architecture**, strictly isolating data between organizations while utilizing a shared, scalable Web3 infrastructure.

```text
📦 PAYPOL OS (Enterprise SaaS)
 ┣ 💻 Client Tier (Browser)
 ┃ ┣ ⚛️ Next.js 14 (React) UI
 ┃ ┣ 🎨 TailwindCSS & Glassmorphism Engine
 ┃ ┗ 🦊 Web3 Provider (MetaMask / WalletConnect)
 ┃
 ┣ ⚙️ Application Logic & SaaS Gateway
 ┃ ┣ 🛣️ Next.js API Route Handlers (REST)
 ┃ ┣ 🛡️ EIP-191 Cryptographic Signature Verifier
 ┃ ┗ 🤖 OpenClaw Agentic Cron-Scheduler (Autopilot)
 ┃
 ┣ 🗄️ Database Tier (Multi-Tenant)
 ┃ ┣ 🗃️ paypol_saas.db (SQLite)
 ┃ ┃ ┣ 🏢 Workspaces (Tenant Isolation)
 ┃ ┃ ┣ 👥 Employee Ledgers & Contacts
 ┃ ┃ ┣ ⏳ Boardroom Approvals Queue
 ┃ ┃ ┗ 📜 Settled Transaction Histories
 ┃
 ┗ 🔗 Blockchain Integration (Tempo Moderato RPC)
   ┣ 🏦 PayPol Time-Vault Logic
   ┣ 🕵️ Solidity ZK-Verifier Contract (Compiled via Noir)
   ┗ 🪙 Native Stablecoins: AlphaUSD, pathUSD, BetaUSD, ThetaUSD
```
---

## 🛠️ Getting Started
### Prerequisites
* Node.js (v18+)
* MetaMask/Rabby extension installed.
* Configure MetaMask with Tempo tesnet (Moderato):
    * RPC URL: https://rpc.moderato.tempo.xyz
    * Chain ID: 42431
### Local Deployment
1. Clone the repository:
   ```bash
   git clone https://github.com/PayPol-Foundation/paypol-protocol.git
   cd paypol-protocol/apps/dashboard/paypol-frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the Master Engine:
   ```bash
   npm run dev
   ```
4. Initialize Genesis Setup:
    * Open http://localhost:3000.
    * Connect your Web3 Wallet.
    * Create your isolated Vault.
    * Note: The first connected wallet becomes the Irreversible Master Administrator for that Workspace.

---

## 🔒 License & Copyright
Business Source License 1.1 (BSL-1.1). See [LICENSE](https://github.com/PayPol-Foundation/paypol-protocol/blob/main/LICENSE) for full terms.

© 2026 PayPol Foundation. All rights reserved.

The source code in this repository is provided for transparency, auditing, and personal educational purposes. Commercial use, production deployment for profit, or forking to create competitive products is strictly prohibited without explicit written permission from the PayPol Foundation.

PayPol OS ensures your hard-earned code remains yours.

---

<div align="center">



<p><b>Built with ❤️ by the PayPol Foundation for a Decentralized Future.</b></p>
</div>

