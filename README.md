# ⛓️ BlockLab — Interactive Blockchain Learning Platform

An interactive, browser-based platform for learning how blockchains work. Build, simulate, and explore blockchain concepts through hands-on experimentation.

**No dependencies. No build step. Pure HTML/CSS/JavaScript.**

![BlockLab](https://img.shields.io/badge/BlockLab-v1.0-blue) ![License](https://img.shields.io/badge/license-MIT-green) ![Deploy](https://img.shields.io/badge/deploy-Vercel-black)

---

## ✨ Features

### 📚 Learn
- **6 Guided Tutorials** with step-by-step interactive walkthroughs that highlight areas of the UI
- **Core Concepts** cards explaining blocks, hashing, proof of work, transactions, decentralization, and immutability
- Keyboard navigation (arrow keys, Escape) for tutorial walkthroughs

### ⛓️ Blockchain Simulator
- Live blockchain visualization with linked blocks
- Add blocks with custom data and watch them get mined
- **Block Inspector** — click any block to view its internals
- **Tamper detection** — edit a block's data and watch the chain invalidate
- Real-time event log

### ⛏️ Mining Lab
- Adjustable difficulty (1-4 leading zeros)
- Real-time proof-of-work visualization
- **Hash Explorer** — type anything and instantly see its SHA-256 hash
- Watch the avalanche effect in action
- Mining console with nonce attempt logging

### 💳 Wallet Simulator
- Create multiple wallets with generated addresses and key pairs
- Send transactions between wallets with digital signatures
- Transaction history with signature verification
- Transactions are recorded as blocks on the chain

### 🌐 Peer Network
- Visual network topology with connected nodes
- Block broadcasting simulation
- **Fork simulation** — watch how consensus resolves competing chains
- Node inspector showing chain state per peer

### 💻 Code Lab
- **6-step progressive tutorial** building a blockchain from scratch
- Runnable code examples with live output
- Copy-paste ready complete implementation (~60 lines)
- Covers: Block class, SHA-256 hashing, chain management, mining, and validation

---

## 🚀 Getting Started

### Run Locally

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/blocklab.git
cd blocklab

# Open directly in browser
open index.html

# Or use any static server
npx serve .
```

### Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Import your GitHub repository
4. Click **Deploy** — no configuration needed!

The included `vercel.json` handles routing automatically.

---

## 🏗️ Project Structure

```
blocklab/
├── index.html      # Entire application (single file)
├── package.json    # Project metadata
├── vercel.json     # Vercel deployment config
└── README.md       # This file
```

The entire app is a single `index.html` file with no external dependencies (except Google Fonts). This makes it:
- **Zero-config** to deploy
- **Instantly loadable** — no build step
- **Easy to learn from** — all the code is right there

---

## 🔧 Technical Details

- **Hashing**: Uses the Web Crypto API (`crypto.subtle.digest`) for real SHA-256
- **Mining**: Genuine proof-of-work implementation with nonce iteration
- **No frameworks**: Pure vanilla JavaScript, CSS, and HTML
- **Responsive**: Works on desktop and mobile
- **No backend**: Everything runs client-side in the browser

---

## 📖 Tutorial System

The guided tutorial system uses a highlight-and-tooltip overlay that:
- Dims the rest of the page
- Highlights the relevant UI element with a glowing border
- Shows explanatory text with next/back navigation
- Automatically navigates between sections
- Supports keyboard shortcuts (←/→ arrows, Escape)

---

## 🎓 Learning Path

1. **Start with Learn** — Read concept cards and pick a guided tutorial
2. **Blockchain Basics** — Understand blocks, chains, and immutability
3. **Cryptographic Hashing** — Experiment with SHA-256 in the Hash Explorer
4. **Mining & Proof of Work** — Mine blocks at different difficulties
5. **Transactions & Wallets** — Create wallets and send signed transactions
6. **Consensus & Network** — See how distributed nodes agree
7. **Build Your Own** — Follow Code Lab to write a blockchain from scratch

---

## 📄 License

MIT — Use freely for education, workshops, courses, and learning.
