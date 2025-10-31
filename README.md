# zkShine Documentation

![Solana](https://img.shields.io/badge/Built_for-Solana-14F195?logo=solana&logoColor=white)
![Docs](https://img.shields.io/badge/Docs-GitBook-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Version-0.3.0--alpha-yellow)

> **zkShine Docs** is the official developer and operator documentation hub — covering ZK Compute, Privacy Relayer, VPN Gateway, SDK, and Node setup for the zkShine ecosystem on **Solana**.

---

## 📘 Overview

zkShine provides a modular zero-knowledge privacy infrastructure for Solana:
- **Developers** can integrate privacy, proofs, and anonymous relays.  
- **Operators** can run zkShine Nodes and earn rewards.  
- **Users** can transact, compute, and communicate privately.

---

## 📚 Documentation Sections

| Section | Description |
|----------|--------------|
| 🧩 [Core Protocol](#core-protocol) | Learn about zkCompute, relayers, and vault design. |
| 🧠 [Developer SDK](#developer-sdk) | Integrate zkShine with your dApps using SDKs. |
| ⚙️ [Node Operator Guide](#node-operator-guide) | Run and configure zkShine Nodes. |
| 💻 [DApp Integration](#dapp-integration) | Use zkShine UI and connect wallets. |
| 🔒 [API Reference](#api-reference) | Learn the REST and GraphQL endpoints. |

---

## 🧩 Core Protocol

zkShine Core powers the proving and verification system.

```console
User → zkCompute Node → Proof → Relay → Solana Program → Vault

Developer SDK

JavaScript SDK allows developers to easily connect their Solana apps to zkShine infrastructure.

import { zkShine } from "@zkshine/sdk";

const zk = await zkShine.init({ network: "devnet" });
await zk.deposit({ from: wallet.publicKey, amount: 1, token: "SOL" });

Node Operator Guide

Learn how to run zkShine Nodes and join the Privacy Network.

Quick Setup
git clone https://github.com/zkshinedev/node.git
cd node
yarn install
yarn start


Or with Docker:

docker compose up -d


More details: Node Docs

💻 DApp Integration

zkShine UI allows users to access private tools on Solana:

Connect Phantom, Backpack, or Solflare wallets

Manage VPN sessions and vault storage

Relay transactions privately

Visit: https://dapps.zkshine.xyz

🔒 API Reference
POST /relay/submit
POST /proof/verify
GET  /vault/fetch


Full list of API endpoints: https://docs.zkshine.xyz/api

🌍 Ecosystem Links
Repo	Purpose
core
	Solana programs & proof logic
sdk-js
	JavaScript SDK
node
	Node infrastructure
ui
	DApp interface
docs
	Documentation & GitBook content
