# ScrapyChain

A blockchain library built from scratch in Rust. Learn blockchain internals by building them.

## What is ScrapyChain?

ScrapyChain is a modular blockchain library that implements core blockchain primitives from the ground up. It's designed to be a hands-on exploration of how blockchains actually work under the hood: hashing, block construction, chain validation, consensus, and beyond.

This isn't a wrapper around existing blockchain frameworks. It's a from-first-principles build using Rust for performance, safety, and the kind of low-level control that blockchain infrastructure demands.

## Current Progress

- [x] **Hashing** - SHA-256 hashing module (using the `sha2` crate) for block and transaction hashing
- [ ] **Block** - Block struct with header, data, timestamp, and hash references
- [ ] **Chain** - Linked chain with validation and integrity checks
- [ ] **Proof of Work** - Mining with adjustable difficulty
- [ ] **Transactions** - Transaction model with inputs/outputs
- [ ] **Persistence** - On-disk storage for chain state
- [ ] **Networking** - P2P node communication (future)

## Getting Started

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) (1.70+)

### Build

```bash
git clone https://github.com/yourusername/scrapy_chain.git
cd scrapy_chain
cargo build
```

### Run Tests

```bash
cargo test
```

## Project Structure

```
scrapy_chain/
├── src/
│   ├── lib.rs          # Library root
│   ├── hash.rs         # SHA-256 hashing utilities
│   ├── block.rs        # Block struct and methods (upcoming)
│   └── chain.rs        # Chain validation (upcoming)
├── tests/              # Integration tests
├── Cargo.toml
└── README.md
```

## Why Rust?

Blockchain infrastructure requires memory safety without garbage collection, predictable performance, and strong type guarantees. That's exactly what Rust provides. Building a blockchain library in Rust isn't just an exercise; it's building with the same language powering Solana, Polkadot, and other production chains.

## Roadmap

**Phase 1: Core Primitives** _(in progress)_
Hashing, blocks, chain linking, and validation.

**Phase 2: Consensus & Mining**
Proof of Work implementation with adjustable difficulty targeting.

**Phase 3: Transactions & State**
UTXO or account-based transaction model, Merkle trees for transaction verification.

**Phase 4: Persistence & Networking**
On-disk chain storage, basic P2P networking between nodes.

## Built By

[Ashutosh akascrapychain](https://github.com/scrapychain) - Software engineer learning blockchain development by building it from scratch. Documenting the journey in public.

## License

MIT
