# PeachSwap Interface

[![Tests](https://github.com/peachswap/peachswap-interface/workflows/Tests/badge.svg)](https://github.com/peachswap/peachswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for PeachSwap -- a protocol for decentralized exchange of Binance Smart Chain BEP20 tokens.

- Website: [peachswap.com](https://peachswap.com/)
- Docs: [uniswap.org/docs/](https://uniswap.org/docs/)
- Twitter: [@PeachSwap](https://twitter.com/PeachSwap)


## Accessing the PeachSwap Interface

To access the PeachSwap Interface, visit [peachswap.com](https://peachswap.com) which is hosted directly on gh-pages branch.

## Listing a token

Please see the
[@peachswapprotocol/default-token-list](https://github.com/peachswapprotocol/default-token-list)
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"`

Note that the interface only works on BSC testnets where both
[PeachSwap Factory & Router Contract](https://github.com/peachswap/contracts/tree/master/contracts) and
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.**
CI checks will run against all PRs.
