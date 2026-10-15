## Raid Ateir

Smart Contract Engineer | DeFi & Blockchain Infrastructure.

📫 ateirraid@gmail.com · 🔗 [deltaflows.xyz](https://deltaflows.xyz)

---

### Selected work — ZKsync (Matter Labs)

**Bridging and token architecture**

- [era-contracts#595](https://github.com/matter-labs/era-contracts/pull/595) — split the monolithic asset router and native token vault into shared base contracts with separate L1/L2 implementations. Foundation for custom bridging logic and L2-native token bridging.
- [era-contracts#1992](https://github.com/matter-labs/era-contracts/pull/1992) — `BaseTokenHolder` contract managing base-token mint and burn, wired into the asset tracker and the V31 upgrade path.
- [zksync-era#4630](https://github.com/matter-labs/zksync-era/pull/4630) — server-side genesis support for the base token holder.
- [era-contracts#772](https://github.com/matter-labs/era-contracts/pull/772) — `GatewayTransactionFilterer`, a whitelist-based filter for transactions routed through the Gateway.

**EIP-7702 bug fix, Protocol upgrades and interop**

- [era-contracts#1654](https://github.com/matter-labs/era-contracts/pull/1654) — EIP-7702 fix: address aliasing and refund-recipient resolution now account for delegated EOAs. Adds `EIP7702Checker` and changes `AddressAliasHelper` and `Mailbox`.
- [era-contracts#1737](https://github.com/matter-labs/era-contracts/pull/1737) — interop library for constructing interop calls.
- [era-contracts#1842](https://github.com/matter-labs/era-contracts/pull/1842) — refactored the interop library to separate per-call from per-bundle attributes, which had been conflated.
- [era-contracts#1664](https://github.com/matter-labs/era-contracts/pull/1664) — automated post-deployment contract verification from deployment logs, replacing a manual per-contract process.

**ZKsync OS — Rust VM**

- [zksync-os#626](https://github.com/matter-labs/zksync-os/pull/626) — FRI precompile and a new transaction type: proofs submitted in the tx sidecar are verified during validation, with validity revealed in-transaction. Enables faster finality for chains settling on Gateway.
- [zksync-os#683](https://github.com/matter-labs/zksync-os/pull/683) — runtime chain config (chain ID, proof verification toggle, gas limits), frozen per batch and committed into the batch public input as a hash. Breaking change to the public-input layout.
- [zksync-os#414](https://github.com/matter-labs/zksync-os/pull/414) — refactored system hooks to delegate validation to system contracts, leaving the hook responsible only for accepting the raw message and emitting events. Paired with [era-contracts#1808](https://github.com/matter-labs/era-contracts/pull/1808).
- [zksync-os#580](https://github.com/matter-labs/zksync-os/pull/580) — made the L2 base-token mint path call the asset tracker explicitly instead of writing its storage slots directly, aligning ZKsync OS with the Era implementation.
- [zksync-os-server#1318](https://github.com/matter-labs/zksync-os-server/pull/1318) — fixed RPC call tracing for L1→L2 transactions with multiple top-level frames, which were previously dropped.

**Developer tooling**

- [zksync-era#4418](https://github.com/matter-labs/zksync-era/pull/4418) — split the monolithic `zkstack ecosystem init` into separate commands for core contracts, new CTM and gateway tx filterer.
- [era-contracts#1648](https://github.com/matter-labs/era-contracts/pull/1648) — restructured the deploy and calldata-generation scripts, mirroring the CLI split on the contracts side.

---

### Personal

- **[deltaflows.xyz](https://deltaflows.xyz)** — concentrated liquidity analytics: tick-level yield comparison across ETH/stablecoin pools on Ethereum and Arbitrum.
