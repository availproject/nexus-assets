# Avail Assets

A repository of blockchain chain and token assets for the Avail ecosystem.

## Structure

```
assets/
├── chains/                    # Blockchain networks
│   ├── _index.json           # Master list of all chains
│   └── {chain}/
│       ├── info.json         # Chain metadata
│       └── logo.png          # Chain logo (256x256 PNG)
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
| Monad | 143 | MON |
| Sophon | 50104 | SOPH |
| Kaia | 8217 | KAIA |
| HyperEVM | 999 | HYPE |
| MegaETH | 4326 | ETH |
| Citrea | 4114 | cBTC |

### Testnets

| Chain | Chain ID | Native Token |
|-------|----------|--------------|
| Ethereum Sepolia | 11155111 | ETH |
| Arbitrum Sepolia | 421614 | ETH |
| OP Sepolia | 11155420 | ETH |
| Polygon Amoy | 80002 | POL |
| Base Sepolia | 84532 | ETH |
| Monad Testnet | 10143 | MON |

## Universal Tokens

| Token | Symbol |
|-------|--------|
| USD Coin | USDC |
| Tether USD | USDT |
| Ethereum | ETH |
| Wrapped Ether | WETH |
| BNB | BNB |
| Avalanche | AVAX |
| Polygon | MATIC |
| POL | POL |
| Kaia | KAIA |
| Monad | MON |
| Hyperliquid | HYPE |
| Citrea BTC | cBTC |
| MegaETH | ETH |
| Sophon | SOPH |

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

## Image Specifications

- **Size**: 256x256 pixels
- **Format**: PNG with transparent background
- **Naming**: `logo.png`

## Usage

### Get chain logo URL

```
https://raw.githubusercontent.com/availproject/nexus-assets/main/chains/{chain}/logo.png
```

### Get token logo URL

```
https://raw.githubusercontent.com/availproject/nexus-assets/main/tokens/{token}/logo.png
```

## License

MIT License

Chain and token logos sourced from [Trust Wallet Assets](https://github.com/trustwallet/assets) (MIT License).
