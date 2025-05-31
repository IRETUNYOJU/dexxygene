# DexxyGene: Decentralized Genetic Data Marketplace

**DexxyGene** is a blockchain-based platform that enables secure, transparent, and permission-controlled sharing of genetic data. Built on the Stacks blockchain using Clarity smart contracts, DexxyGene creates a decentralized marketplace where genetic data owners can monetize their assets, while researchers gain verifiable and time-bound access to valuable genetic information.

---

## 🔑 Key Features

* **Secure Data Ownership**
  Genetic data owners retain full control over their data assets at all times.

* **Tiered Access Levels**
  Customizable access tiers to accommodate diverse research needs and compliance requirements.

* **Time-Limited Access**
  Smart contracts enforce automatic expiration of access rights after a specified duration.

* **Verifiable Transactions**
  All access and data transactions are transparently recorded on-chain.

* **Privacy-Preserving**
  Only hashed metadata is stored on-chain, ensuring sensitive data remains private and secure.

---

## 🧠 Smart Contracts Overview

DexxyGene includes two core Clarity smart contracts:

* `gene-asset-trait.clar`: Defines the interface and structure for genetic data assets.
* `gene-market.clar`: Implements the decentralized marketplace functionality.

---

## ⚙️ How It Works

1. **Asset Registration**
   Data owners register their genetic data with associated metadata and pricing.

2. **Discovery**
   Researchers browse the catalog of available genetic datasets.

3. **Purchase Access**
   Researchers purchase time-limited access to specific genetic data.

4. **Verification**
   Smart contracts verify access rights during data requests.

5. **Automatic Expiry**
   Access permissions automatically expire after the specified time period.

---

## 🚀 Getting Started

### Prerequisites

* [Clarinet](https://docs.stacks.co/docs/clarity/clarinet) for local smart contract development
* [Stacks Wallet](https://wallet.hiro.so/) for contract deployment and interaction

---

### 📥 Installation

Clone the DexxyGene repository:

```bash
git clone https://github.com/fhayvy/genedex.git
cd genedex
```

Install dependencies:

```bash
npm install
```

Run tests:

```bash
clarinet test
```

---

## 🧬 Usage

### For Data Owners

```clarity
;; Register a new genetic data asset
(contract-call? .gene-market register-asset u1000 0x012345...)
```

### For Researchers

```clarity
;; Purchase access to a genetic data asset
(contract-call? .gene-market purchase-access u1 u2)
```

### For Administrators

```clarity
;; Set a new curator for moderation or governance
(contract-call? .gene-market set-curator 'ST1PQHQKV0RJXZFY1DGX8MNSNYVE3VGZJSRTPGZGM)
```

---

## 🛤️ Roadmap

* ✅ Integration with off-chain storage systems (e.g., IPFS, Arweave)
* 🔐 Enhanced privacy with zero-knowledge proofs
* 📱 Mobile application for user-friendly access
* 🔌 RESTful API for third-party integration and data analytics platforms

---

## 🤝 Contributing

We welcome contributions from developers, geneticists, and privacy advocates! Feel free to fork the project, submit issues, or open a pull request.

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---


