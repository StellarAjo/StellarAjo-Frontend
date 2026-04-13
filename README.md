# StellarAjo-Frontend


> **Mobile-first interface for blockchain-secured Susu groups.**
The StellarSusu App is a **React Native (Expo)** mobile application that provides a simple, familiar interface for interacting with the **SoroSusu smart contract** on the Stellar network.

It transforms complex blockchain interactions into an experience that feels like using a messaging or group savings app — accessible to everyday users across Africa and the diaspora.

---

## 🌍 What This App Does

The app enables users to:

* Create and manage Susu (Ajo, Chama, Stokvel) groups
* Contribute funds securely via blockchain
* Receive payouts automatically based on group cycles
* Track all transactions transparently

All without needing to understand how blockchain works.

---

## ✨ Core Features

### 👥 Group Management

* Create a new Susu group in minutes
* Join groups via invite link or QR code
* View member list and payout order

### 💸 Contributions & Payouts

* Make scheduled contributions
* Automatic payout when it’s your turn
* Real-time status of current cycle

### 🔔 Notifications

* Contribution reminders
* Payout alerts
* Group activity updates

### 🌐 Localization

* Multi-language support (English, Yoruba, Swahili, etc.)
* Local currency display

---

## 🔐 Security & Trust

* **Non-custodial:** Users control their wallets
* **On-chain logic:** All rules enforced by smart contract
* **Transparent:** Every transaction is visible
* **Immutable:** Records cannot be altered

---

## 🧱 Architecture (Frontend)

```
Mobile App (React Native + Expo)
        │
        ▼
StellarSusu SDK (TypeScript)
        │
        ▼
Soroban Smart Contract (Stellar Network)
```

---

## ⚙️ Tech Stack

| Category           | Technology                         |
| ------------------ | ---------------------------------- |
| Framework          | React Native + Expo                |
| Styling            | NativeWind (Tailwind CSS for RN)   |
| State Management   | Zustand                            |
| Data Fetching      | React Query                        |
| Blockchain SDK     | @stellar/stellar-sdk               |
| Wallet Integration | Freighter, WalletConnect, Passkeys |
| Optional Backend   | Supabase                           |

---

## 🚀 Getting Started

### Prerequisites

* Node.js (v18+)
* Expo CLI

  ```bash
  npm install -g expo-cli
  ```
* A Stellar testnet wallet:

  * Freighter (browser)
  * Lobstr (mobile)

---

### 📦 Installation

```bash
git clone https://github.com/stellarsusu/stellarsusu-app.git
cd stellarsusu-app

npm install
```

---

### 🔧 Environment Setup

```bash
cp .env.example .env
```

Add:

* Stellar RPC URL
* Network passphrase (testnet)

---

### ▶️ Run the App

```bash
npm run start
```

---

### 📱 Run on Device

```bash
# iOS
npm run ios

# Android
npm run android
```

---

## 🔗 Key App Flows

### Create Group

1. Enter contribution amount
2. Set cycle length
3. Invite members

### Join Group

* Open invite link or scan QR code
* Connect wallet
* Confirm participation

### Contribute

* Approve transaction from wallet
* Funds locked in smart contract

### Receive Payout

* Automatically sent when your cycle arrives

---

## 🔌 Smart Contract Integration

The app interacts with the SoroSusu protocol via the SDK.

| Action         | Contract Function |
| -------------- | ----------------- |
| Create group   | `create_group`    |
| Join group     | `join_group`      |
| Contribute     | `contribute`      |
| Receive payout | `disburse`        |
| View state     | `get_group_state` |

---

## 📂 Project Structure

```
stellarsusu-app/
├── app/                # Screens & navigation
├── components/         # Reusable UI components
├── hooks/              # Custom hooks
├── store/              # Zustand state
├── services/           # API / blockchain interactions
├── sdk/                # Contract interaction layer
├── assets/             # Images, fonts
└── utils/              # Helpers
```

---

## 🧪 Testing

* Manual testing on Android & iOS devices
* Focus on low-end Android performance
* Wallet interaction testing (Freighter, Lobstr)

---

## 🤝 Contributing

We welcome contributions from developers, designers, and community members.

### How to Contribute

1. Fork the repo
2. Create a feature branch
3. Submit a PR



## 🗺️ Roadmap

* ✅ Group creation & contribution flow
* 🔄 Wallet onboarding improvements
* 🔜 Mainnet release
* 🔮 Savings goals & analytics
* 🔮 Remittance integrations

