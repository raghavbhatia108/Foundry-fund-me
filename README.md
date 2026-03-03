# 💰 Foundry Fund Me

A crowdfunding smart contract built with **Solidity** and **Foundry**.  
Users can fund the contract with ETH, and only the owner can withdraw the funds.

This project demonstrates:

- Solidity smart contract development
- Chainlink price feed integration
- Foundry unit & integration testing
- Deployment scripts
- Makefile automation

---

## 🛠 Tech Stack

- Solidity ^0.8.18
- Foundry
- Chainlink Price Feeds
- Forge Std

---

## 📂 Project Structure

```
foundry-fundMe/
│
├── src/
│   ├── FundMe.sol              # Main crowdfunding contract
│   └── PriceConverter.sol      # Chainlink price conversion library
│
├── script/
│   ├── DeployFundMe.s.sol      # Deployment script
│   ├── HelperConfig.s.sol      # Network configuration helper
│   └── Interactions.s.sol      # Fund & Withdraw interaction scripts
│
├── test/
│   ├── unit/
│   │   └── FundMeTest.t.sol        # Unit tests
│   │
│   ├── integration/
│   │   └── InteractionsTest.t.sol  # Integration tests
│   │
│   └── mocks/
│       └── MockV3Aggregator.sol    # Mock Chainlink price feed
│
├── lib/                        # Dependencies (forge-std, chainlink, etc.)
├── foundry.toml                # Foundry configuration
├── foundry.lock                # Dependency lock file
├── Makefile                    # Automation commands
└── README.md                   # Project documentation
```