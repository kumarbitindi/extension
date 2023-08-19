<br /> 
<p align="center">
  <a href="https://bitindi.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/11839151/188500975-8cd95d07-c419-48aa-bb85-4200a6526f68.svg" />
      <source media="(prefers-color-scheme: light)" srcset="https://blockwallet.io/static/images/logo-blockwallet-black.svg" />
      <img src="[https://blockwallet.io/static/images/logo-medium.svg](https://user-images.githubusercontent.com/11839151/188500975-8cd95d07-c419-48aa-bb85-4200a6526f68.svg)" width="300" />
    </picture>
  </a>
</p>

<div align="center" style="text-align:center">

[![CI](https://github.com/block-wallet/extension/actions/workflows/ci.yml/badge.svg)](https://github.com/block-wallet/extension/actions/workflows/ci.yml) [![Release (manual)](https://github.com/block-wallet/extension/actions/workflows/build.yml/badge.svg)](https://github.com/block-wallet/extension/actions/workflows/build.yml) [![Release (automated)](https://github.com/block-wallet/extension/actions/workflows/release.yml/badge.svg)](https://github.com/block-wallet/extension/actions/workflows/release.yml)

</div>

<hr />

# Bitindi Wallet - Extension

The most private, non-custodial cryptocurrency wallet
The first crypto wallet protects you on Web3 without any compromises. Stay safe with BlockWallet.

Supporting Ethereum, BNB Chain, Polygon, Avalanche, Fantom, and Arbitrum.

BlockWallet is for you if:

- You frequently use DApps and DEXes.
- You want your tools working smoothly, every time.
- You care about your personal data and security online.
- You are tired of overly-cluttered and confusing crypto wallets.

## Getting Started

See the [guideline](docs/guideline.md)

### Prerequisites

- Node.js: version at [.nvmrc](.nvmrc)
- Yarn
- Make

### Installing

#### Environment

It's also needed to setup the environment variables on each package. In both `~/packages/background` and `~/packages/provider`, copy the contents of `env.orig` file into a new file called `.env`.

They should look like:

**packages/background/.env**

```
// Complete with the corresponding keys.
ETHERSCAN_API_KEY= // Included in requests to Etherscan. Can be obtained in https://etherscan.io/apis.
```

**packages/provider/.env**

```
LOG_LEVEL=error
```

#### Install

To install all the dependencies run the command

```
make install
```

### Build

Once you installed everything run the command

```
make build
```

### Running the tests

Once you build the extension run the command

```
make test
```

### Coding style

Every [package](packages) has it own coding style. In order to check the styles run the command

```
make lint
```
## Built With

- [Node.js](https://nodejs.org/)
- [Typescript](https://www.typescriptlang.org/)
- [React.js](https://reactjs.org/)
- [tailwindcss](https://tailwindcss.com/)


## License

See the [LICENSE](LICENSE) file for details
