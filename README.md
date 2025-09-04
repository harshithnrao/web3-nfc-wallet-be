# Web3 NFC Wallet Backend

> A NestJS-based backend powering an NFC-enabled Ethereum wallet.  
> Designed to simplify blockchain interactions for a Flutter frontend using MetaMask and Etherscan.

---

## 🚀 Overview

This project is the backend API for a mobile crypto wallet that enables **NFC-based Ethereum transactions**.  
Built with **NestJS** and **TypeScript**, the backend communicates with **MetaMask** and **Etherscan APIs** to:

- Fetch wallet balances
- Retrieve transaction history
- Estimate gas prices
- Initiate transactions

No database is used—this backend interacts **directly with the Ethereum blockchain** to ensure real-time data accuracy and decentralized architecture.

---

## 🔧 Tech Stack

- **Node.js + TypeScript**
- **NestJS** – Scalable backend framework
- **Ethers.js** – Ethereum blockchain interaction
- **MetaMask** – Wallet integration
- **Etherscan API** – Transaction and balance data


---

## 📱 Real-World Use Case

The backend is built for a **Flutter-based mobile wallet** that allows users to:

- Tap an NFC card to sign/authorize Ethereum transactions
- View live ETH balance and transaction history
- Estimate gas before sending
- Interact with smart contracts via MetaMask

This design ensures the **Flutter frontend remains lightweight** while delegating complex blockchain interactions to this service.

---

## 🔄 API Capabilities

| Endpoint                         | Description                          |
|----------------------------------|--------------------------------------|
| `GET /balance/:address`          | Fetch ETH balance for wallet address |
| `GET /transactions/:address`     | Retrieve transaction history         |
| `GET /gas-price`                 | Get current gas prices               |
| `POST /send-transaction`         | Initiate/send ETH transaction        |

*(All routes and params are illustrative—see code for implementation details.)*

---
## 🔐 Environment Setup

To run this project, you'll need to create a `secret.json` file in the root directory with your API keys:

```json
{
  "metamask_api_key": "YOUR_INFURA_OR_ALCHEMY_KEY",
  "etherscan_api_key": "YOUR_ETHERSCAN_KEY"
}
```
---
## 🧪 Running Locally

### Install dependencies

```bash
npm install

# development
npm run start

# watch mode
npm run start:dev

# production
npm run start:prod
```

🧠 What I Learned

How to structure a modular backend with NestJS

Using Ethers.js for secure blockchain interactions

Designing API-first backend for frontend simplicity

Writing clean, testable code with TypeScript

Architecting a no-DB solution for decentralized apps


📌 Future Enhancements

Add support for other EVM chains (e.g., Polygon, BSC)

Secure API with rate limiting and auth

Add Swagger/OpenAPI documentation

Extend support for ERC20 tokens


🧑‍💻 Author

Harshith N Rao | 
Software Developer | 
https://github.com/harshithnrao

⚠️ This project is a work-in-progress. Actively seeking feedback and collaboration.
