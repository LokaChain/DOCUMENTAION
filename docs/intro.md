---
sidebar_position: 1
---

# 📖 Introduction
Welcome to the documentation of LokaChain. This guide will help developers, validators, and users understand and interact with the chain.

# Setup Instructions

## 1. Install Prerequisites
 You need the following tools installed:

- **Go** (version 1.20 or higher)
- **Git**
- **Make** (optional, but recommended)


### Install Go
- Follow the official Go installation guide or use Homebrew (on macOS):
```bash
 brew install go
```
### Install Git
```bash
 brew install git
```
## 2. Clone the Blockchain Repository
```bash
git clone https://github.com/LokaChain
cd LokaChain
```

## Compiling the blockchain

To compile the source code of a  Lokachain application into a runnable binary, effectively creating a local executable for your blockchain

```bash
ignite chain build
```

# Start a full node
```bash
 ~/go/bin/lokachaind start
```
Breakdown :
- `~/go/bin/lokachaind`:This is the binary executable for your custom Lokachain application, located in the Go binary path (~/go/bin).

- `~/go/bin/lokachaind`:This is the binary executable for your custom LokaChain application, located in the Go binary path (~/go/bin).

- `start`:This subcommand starts the Tendermint consensus engine and ABC I application, which together run your node
