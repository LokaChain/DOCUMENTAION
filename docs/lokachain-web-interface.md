---
title: "🌐 Lokachain Web Interface"
---

# 🌐 Lokachain Web Interface

This is the frontend interface for interacting with the **Lokachain** blockchain, built on the Cosmos SDK. It allows users to:

- Add a chain to Keplr
- Check their address and balance
- Send tokens
- Initialize CosmWasm client
- Run useful CLI commands

---

##  Development Notes

###  Dependencies
-**Keplr Wallet**
-**Cosmos SDK**
-**REST/RPC Endpoints**

###  Account Setup
- Keplr generates new accounts from your seed.
- Pre-funded accounts:
  - `alice` (~20M STAKE)
  - `bob` (~100 STAKE)
- You can transfer tokens from `alice`/`bob` to your Keplr address for testing.

###  Troubleshooting
- Check browser console (`F12`) for detailed logs.
- Ensure **Keplr** is installed and unlocked.
- Verify RPC/REST endpoints are accessible.
- Ensure your blockchain is running.
- Try refreshing the page if issues persist.

### ⚙️ Gas Configuration
| Level    | Gas Value         |
|----------|-------------------|
| Low      | `0.01 STAKE/gas`  |
| Average  | `0.025 STAKE/gas` |
| High     | `0.04 STAKE/gas`  |

---

##  Send Tokens

Use the form to transfer tokens:

- **Recipient Address:** Paste or enter manually.
- **Amount:** Enter amount in STAKE (fee: ~0.005 STAKE).

---

## 🛠️ Smart Contracts

Click **"Initialize CosmWasm Client"** to connect with smart contract modules.

---

##  Useful CLI Commands

### ➤ Transfer Tokens
```bash
lokachaind tx bank send alice [ADDRESS] 1000000stake --chain-id lokachain
``` 

### ➤Check balance
```bash
lokachaind query bank balances [ADDRESS]
``` 

##  Status Bar
- **Connection Status** : Shows if Keplr and RPC are connected.
- **Buttons**:
-Add Chain: Add Lokachain to Keplr

-Check: Check current wallet connection

-Test RPC: Verify RPC functionality

-Get Address: Retrieve wallet address

-Refresh Balance: Update token balance
