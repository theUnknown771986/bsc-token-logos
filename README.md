# BSC Token Logos Registry (Chain ID 56)

Official logo registry for BNB Smart Chain tokens — wallet-ready images served from raw.githubusercontent.com for use in any wallet platform (MetaMask, Trust Wallet, TokenPocket, MathWallet, frontends, explorers).

## Structure (ethereum-lists/tokens compatible)

```
assets/<contract-address>/
  logo.png   # official logo
  info.json  # name, website, shortName, decimals
native/
  BNB.png    # native coin logo
bsc.tokenlist.json   # Uniswap-standard token list (with logoURI per token)
logos.json           # simple manifest
```

## Tokens included

| Symbol | Name | Address |
|---|---|---|
| WBNB | Wrapped BNB | `0xbb4CdB9CBd36B01bD1cBaEBF2De08d9173bc095c` |
| USDT | Binance-Peg BSC-USD Token | `0x55d398326f99059fF775485246999027B3197955` |
| BUSD | Binance USD | `0xe9e7CEA3DedcA5984780Bafc599bD69ADd087D56` |
| USDC | Binance-Peg USD Coin | `0x8AC76a51cc950d9822D68b83fE1Ad97B32Cd580d` |
| CAKE | PancakeSwap Token | `0x0E09FaBB73Bd3Ade0a17ECC321fD13a19e81cE82` |

## Use in any wallet / dApp

**Logo URL pattern** (this is all a wallet needs):

```
https://raw.githubusercontent.com/theUnknown771986/bsc-token-logos/main/assets/<CONTRACT_ADDRESS>/logo.png
```

**Uniswap-style list** (import into any dApp supporting token lists):

```
https://raw.githubusercontent.com/theUnknown771986/bsc-token-logos/main/bsc.tokenlist.json
```

**Simple manifest:**

```
https://raw.githubusercontent.com/theUnknown771986/bsc-token-logos/main/logos.json
```

**MetaMask-style lookup example:**

```js
const logoUrl = `https://raw.githubusercontent.com/theUnknown771986/bsc-token-logos/main/assets/${tokenAddress}/logo.png`;
```

## Adding a token

1. Create `assets/<checksummed-address>/`
2. Add `logo.png` (PNG, ~256x256, official brand art)
3. Add `info.json`: `{"name", "website", "shortName", "decimals"}`
4. Open a PR — include the source of the logo in the description

> Logos sourced from [trustwallet/assets](https://github.com/trustwallet/assets) and official project sites. If a project wants its logo updated, open an issue.

Companion repo: [bsc-chain-registry](https://github.com/theUnknown771986/bsc-chain-registry) — chain 56 metadata (RPCs, explorers, EIP-155 entry).
