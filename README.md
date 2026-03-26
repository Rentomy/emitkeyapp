# emitkey — Ethereum Paper Wallet Generator

> Generate secure Ethereum paper wallets — 100% in your browser, 100% offline, 100% open source.

**[emitkey.com](https://www.emitkey.com)** · [How it works](https://www.emitkey.com/how-it-works) · [Security Guides](https://www.emitkey.com/guides)

---

## What is emitkey?

emitkey is a free, open-source Ethereum paper wallet generator that runs entirely in your browser. No server, no account, no tracking. Your private key is generated locally and never transmitted anywhere.

A paper wallet generated on emitkey.com works on **every EVM-compatible network** — Ethereum, Polygon, BNB Chain, Arbitrum, Optimism, Base, Avalanche, and more. Same private key. Same address. Always.

---

## Features

- **Generate Wallet** — Instantly create a secure Ethereum wallet with public address and private key
- **Vanity Address** — Search for a custom address prefix (e.g. `0xDEAD...`)
- **Batch Generator** — Create up to 100 wallets at once, export as CSV or PDF
- **Verify Wallet** — Confirm your private key correctly derives your public address — locally, no internet needed
- **Print / Save PDF** — Export a clean paper wallet with QR codes for cold storage
- **Works Offline** — Install as a PWA and use completely air-gapped after first load
- **EVM Compatible** — Works on Ethereum, Polygon, BNB Chain, Arbitrum, Optimism, Base, and all EVM networks
- **Open Source** — Fully auditable. No hidden code, no dependencies on emitkey.com

---

## Security

- All wallet generation happens in your browser via [ethers.js v6](https://docs.ethers.org/)
- Private keys are derived using the `secp256k1` elliptic curve standard — the same used by Ethereum and Bitcoin
- No data is stored, logged, or transmitted
- The site works fully offline after the first load — disconnect from the internet before generating your wallet for maximum security
- Your paper wallet is **completely independent of emitkey.com** — even if this site shuts down, your private key works on Ethereum forever

> For a full explanation of the cryptography behind Ethereum wallets, visit [emitkey.com/how-it-works](https://www.emitkey.com/how-it-works)

---

## Getting Started

### Use online

Visit **[emitkey.com](https://www.emitkey.com)**, disconnect from the internet, and generate your wallet.

### Install as PWA (recommended)

Visit emitkey.com in your browser and install it as an app — it will work fully offline after installation.

### Run locally

```bash
# Clone the repository
git clone https://github.com/Rentomy/emitkey.git
cd emitkey

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for production

```bash
npm run build
npm start
```

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| [Next.js 15](https://nextjs.org/) | React framework |
| [ethers.js v6](https://docs.ethers.org/) | Wallet generation & cryptography |
| [qrcode](https://www.npmjs.com/package/qrcode) | QR code generation for print/PDF |
| [qrcode.react](https://www.npmjs.com/package/qrcode.react) | QR code display in browser |
| [Tailwind CSS](https://tailwindcss.com/) | Styling |
| [TypeScript](https://www.typescriptlang.org/) | Type safety |

---

## Supported Networks

A wallet generated on emitkey works on all EVM-compatible networks:

| Network | Ticker |
|---------|--------|
| Ethereum | ETH |
| Polygon | MATIC |
| BNB Chain | BNB |
| Arbitrum | ARB |
| Optimism | OP |
| Avalanche (C-Chain) | AVAX |
| Base | BASE |
| zkSync | ZK |
| and all EVM networks... | |

---

## Guides

emitkey includes three security guides for safely using paper wallets:

- **[Cold Storage](https://www.emitkey.com/guides)** — How to store your crypto securely forever
- **[Time-Lock](https://www.emitkey.com/guides)** — How to lock funds until a future date, without a smart contract
- **[Inheritance Wallet](https://www.emitkey.com/guides)** — How to ensure your crypto can be inherited — using only paper

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

Free to use, modify, and distribute.

---

## Contributing

Contributions are welcome. Please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## Disclaimer

emitkey.com is provided as-is, without warranty of any kind. Always verify your wallet before storing significant funds. Never share your private key with anyone. The developers are not responsible for any loss of funds.

---

## Support

If emitkey has been useful to you, consider giving it a ⭐ on GitHub — it helps others find the project.

---

*Built with ♦ by [Rentomy](https://github.com/Rentomy)*
