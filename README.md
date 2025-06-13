# DexPort

**DexPort** is a cross-chain decentralized exchange (DEX) frontend built with Next.js, TypeScript, RainbowKit, and Wagmi. It provides a sleek interface for users to connect wallets and swap tokens across EVM-compatible blockchains such as Ethereum, Polygon, Cronos, Arbitrum, Base, and more.

---

## 📸 Dashboard Preview

![Dashboard Screenshot](./public/images/dashboard.png)

> A clean, modern dashboard for multi-chain token swaps with wallet integration and real-time interaction.

---

## ✨ Features

- 🔗 **Multi-Chain Support**: Ethereum, Polygon, Cronos, Arbitrum, Base, Sepolia
- 🦄 **Wallet Integration**: MetaMask, WalletConnect, Rainbow, etc.
- ⚙️ **Dynamic ABIs**: Loads token and contract ABIs for interacting with smart contracts
- ⚡ **React + TypeScript**: Built with Next.js and type-safe hooks
- 🌐 **Server-Side Rendering (SSR)**: Fast, web3-ready app rendering

---

## 🧱 Tech Stack

- **Next.js** – Web app framework
- **TypeScript** – Type safety
- **RainbowKit** – Wallet UI
- **Wagmi** – Ethereum hooks
- **Ethers.js** – Smart contract interaction
- **JSON ABIs** – Token contract definitions

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/aimaster-dev/dexport.git
cd dexport
````

### 2. Install dependencies

```bash
npm install
```

### 3. Create `.env.local`

```env
NEXT_PUBLIC_ENABLE_TESTNETS=true
NEXT_PUBLIC_PROJECT_ID=your_walletconnect_project_id
```

> 🔑 Get your WalletConnect Project ID at: [https://cloud.walletconnect.com](https://cloud.walletconnect.com)

### 4. Run the development server

```bash
npm run dev
```

---

## 🔗 Chains

DexPort currently supports the following networks:

* Ethereum Mainnet
* Polygon
* Arbitrum
* Cronos
* Base
* Sepolia (testnet, optional)

To enable testnets, make sure your `.env.local` includes:

```env
NEXT_PUBLIC_ENABLE_TESTNETS=true
```

---

## 📦 ABI Management

ABIs are stored in `src/abis/` and dynamically loaded based on token name:

```ts
import { getAbi } from '@/utils/abis';

const abi = getAbi({ name: 'USDC', address: '0x...' });
```

---

## 📜 License

MIT License

---

## 🔗 Repository

GitHub: [https://github.com/aimaster-dev/dexport](https://github.com/aimaster-dev/dexport)
