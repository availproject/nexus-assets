# Avail Assets

A repository of blockchain chain and token assets for the Avail ecosystem.

## Structure

```
assets/
├── chains/                    # Blockchain networks
│   ├── _index.json           # Master list of all chains
│   └── {chain}/
│       ├── info.json         # Chain metadata
│       ├── logo.png          # Chain logo (256x256 PNG)
│       └── assets/           # Chain-specific tokens (optional)
│           └── {address}/
│               ├── info.json
│               └── logo.png
│
└── tokens/                    # Cross-chain token definitions
    ├── _index.json           # Master token list
    └── {token}/
        ├── info.json         # Token metadata
        └── logo.png          # Universal token logo
```

## Supported Chains

### Mainnets

| Chain | Chain ID | Native Token |
|-------|----------|--------------|
| Ethereum | 1 | ETH |
| Arbitrum | 42161 | ETH |
| Optimism | 10 | ETH |
| Polygon | 137 | POL |
| Base | 8453 | ETH |
| Scroll | 534352 | ETH |
| Avalanche | 43114 | AVAX |
| BNB Smart Chain | 56 | BNB |
| Monad | TBD | MON |
| Sophon | TBD | SOPH |
| Kaia | 8217 | KAIA |
| HyperEVM | TBD | HYPE |

### Testnets

| Chain | Chain ID | Native Token |
|-------|----------|--------------|
| Ethereum Sepolia | 11155111 | ETH |
| Arbitrum Sepolia | 421614 | ETH |
| OP Sepolia | 11155420 | ETH |
| Polygon Amoy | 80002 | POL |
| Base Sepolia | 84532 | ETH |
| Monad Testnet | TBD | MON |

## Universal Tokens

| Token | Symbol |
|-------|--------|
| USD Coin | USDC |
| Tether USD | USDT |
| Ethereum | ETH |

## File Formats

### Chain info.json

```json
{
  "name": "Ethereum Mainnet",
  "chainId": 1,
  "symbol": "ETH",
  "decimals": 18,
  "type": "mainnet",
  "explorer": "https://etherscan.io"
}
```

### Token info.json

```json
{
  "name": "USD Coin",
  "symbol": "USDC",
  "website": "https://www.circle.com/usdc",
  "description": "A fully collateralized US dollar stablecoin"
}
```

### Per-chain token asset info.json

```json
{
  "name": "USD Coin",
  "symbol": "USDC",
  "decimals": 6,
  "address": "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48",
  "type": "ERC20"
}
```

## Image Specifications

- **Size**: 256x256 pixels
- **Format**: PNG with transparent background
- **Naming**: `logo.png`

## Usage

### Get chain logo URL

```
https://raw.githubusercontent.com/{owner}/assets/main/chains/{chain}/logo.png
```

### Get token logo URL

```
https://raw.githubusercontent.com/{owner}/assets/main/tokens/{token}/logo.png
```

## License

MIT License

Chain and token logos sourced from [Trust Wallet Assets](https://github.com/trustwallet/assets) (MIT License).
